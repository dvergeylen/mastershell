---
layout: default
title: "phpspec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpspec">
  <a href="/en/common/phpspec.html">phpspec</a> <a href="#phpspec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A Behaviour Driven Development tool for PHP.
> More information: <https://phpspec.net>.

#### Create a specification for a class:
```shell
phpspec describe {{class_name}}
```
#### Run all specifications in the "spec" directory:
```shell
phpspec run
```
#### Run a single specification:
```shell
phpspec run {{path/to/class_specification_file}}
```
#### Run specifications using a specific configuration file:
```shell
phpspec run -c {{path/to/configuration_file}}
```
#### Run specifications using a specific bootstrap file:
```shell
phpspec run -b {{path/to/bootstrap_file}}
```
#### Disable code generation prompts:
```shell
phpspec run --no-code-generation
```
#### Enable fake return values:
```shell
phpspec run --fake
```
{% endraw %}