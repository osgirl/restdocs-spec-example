# Example using restdocs-spec-maven-plugin

[![Build Status](https://travis-ci.org/BerkleyTechnologyServices/restdocs-spec-example.svg?branch=master)](https://travis-ci.org/BerkleyTechnologyServices/restdocs-spec-example)

This example project demonstrates how to integrate [Spring REST Docs], [restdocs-openapi], and the 
[restdocs-spec-maven-plugin] to generate both HTML documentation and an OpenAPI 2.0 spec file at the 
same time.

## Usage

You can build the project with the following command:

```sh
./mvnw clean prepare-package 
```

That should produce the following:

* `./target/classes/static/docs/openapi-2.0.yml` - An OpenAPI 2.0 specification file for the API
* `./target/classes/static/docs/index.hmtl` - The HTML documentation for the API.  This documentation 
  also includes a link to download the OpenAPI 2.0 specification file mentioned above.

[Spring REST Docs]: https://spring.io/projects/spring-restdocs
[restdocs-openapi]: https://github.com/ePages-de/restdocs-openapi
[restdocs-spec-maven-plugin]: https://github.com/BerkleyTechnologyServices/restdocs-spec