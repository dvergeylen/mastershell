---
layout: default
title: "license"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="license">
  <a href="/en/common/license.html">license</a> <a href="#license"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create license files for open-source projects.
> More information: <https://nishanths.github.io/license>.

#### Print a license to stdout, using the defaults (auto-detected author name, and current year):
```shell
license {{license_name}}
```
#### Generate a license and save it to a file:
```shell
license -o {{filename}} {{license_name}}
```
#### List all available licenses:
```shell
license ls
```
#### Generate a license with custom author name and year:
```shell
license --name {{author}} --year {{release_year}} {{license_name}}
```
{% endraw %}