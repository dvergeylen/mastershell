---
layout: default
title: "swagger-codegen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="swagger-codegen">
  <a href="/en/common/swagger-codegen.html">swagger-codegen</a> <a href="#swagger-codegen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate code and documentation for your REST api from a OpenAPI/swagger definition.
> More information: <https://github.com/swagger-api/swagger-codegen>.

#### Generate documentation and code from an OpenAPI/swagger file:
```shell
swagger-codegen generate -i {{swagger_file}} -l {{language}}
```
#### Generate java code using the library retrofit2 and the option useRxJava2:
```shell
swagger-codegen generate -i {{http://petstore.swagger.io/v2/swagger.json}} -l {{java}} --library {{retrofit2}} -D{{useRxJava2}}={{true}}
```
#### List available languages:
```shell
swagger-codegen langs
```
#### Display help options for the generate command:
```shell
swagger-codegen help {{generate}}
```
{% endraw %}