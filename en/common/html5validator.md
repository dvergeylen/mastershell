---
layout: default
title: "html5validator"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="html5validator">
  <a href="/en/common/html5validator.html">html5validator</a> <a href="#html5validator"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for testing HTML5 validity.
> More information: <https://github.com/svenkreiss/html5validator>.

#### Validate a specific file:
```shell
html5validator {{path/to/file}}
```
#### Validate all HTML files in a specific directory:
```shell
html5validator --root {{path/to/directory}}
```
#### Show warnings as well as errors:
```shell
html5validator --show-warnings {{path/to/file}}
```
#### Match multiple files using a glob pattern:
```shell
html5validator --root {{path/to/directory}} --match "{{*.html *.php}}"
```
#### Ignore specific directory names:
```shell
html5validator --root {{path/to/directory}} --blacklist "{{node_modules vendor}}"
```
#### Output the results in a specific format:
```shell
html5validator --format {{gnu|xml|json|text}} {{path/to/file}}
```
#### Output the log at a specific verbosity level:
```shell
html5validator --root {{path/to/directory}} --log {{debug|info|warning}}
```
{% endraw %}