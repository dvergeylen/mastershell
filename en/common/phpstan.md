---
layout: default
title: "phpstan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpstan">
  <a href="/en/common/phpstan.html">phpstan</a> <a href="#phpstan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP static analysis tool to discover bugs in code.
> More information: <https://github.com/phpstan/phpstan>.

#### Display available options for analysis:
```shell
phpstan analyse --help
```
#### Analyse the specified space-separated directories:
```shell
phpstan analyse {{path/to/directory}}
```
#### Analyse a directory using a configuration file:
```shell
phpstan analyse {{path/to/directory}} --configuration {{path/to/config}}
```
#### Analyse using a specific rule level (0-7, higher is stricter):
```shell
phpstan analyse {{path/to/directory}} --level {{level}}
```
#### Specify an autoload file to load before analysing:
```shell
phpstan analyse {{path/to/directory}} --autoload-file {{path/to/autoload_file}}
```
#### Specify a memory limit during analysis:
```shell
phpstan analyse {{path/to/directory}} --memory-limit {{memory_limit}}
```
{% endraw %}