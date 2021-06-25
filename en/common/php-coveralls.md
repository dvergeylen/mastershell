---
layout: default
title: "php-coveralls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="php-coveralls">
  <a href="/en/common/php-coveralls.html">php-coveralls</a> <a href="#php-coveralls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP client for Coveralls.
> More information: <https://php-coveralls.github.io/php-coveralls>.

#### Send coverage information to Coveralls:
```shell
php-coveralls
```
#### Send coverage information to Coveralls for a specific directory:
```shell
php-coveralls --root_dir {{path/to/directory}}
```
#### Send coverage information to Coveralls with a specific config:
```shell
php-coveralls --config {{path/to/.coveralls.yml}}
```
#### Send coverage information to Coveralls with verbose output:
```shell
php-coveralls --verbose
```
#### Send coverage information to Coveralls excluding source files with no executable statements:
```shell
php-coveralls --exclude-no-stmt
```
#### Send coverage information to Coveralls with a specific environment name:
```shell
php-coveralls --env {{test|dev|prod}}
```
#### Specify multiple Coverage Clover XML files to upload:
```shell
php-coveralls --coverage_clover {{path/to/first_clover.xml}} --coverage_clover {{path/to/second_clover.xml}}
```
#### Output the JSON that will be sent to Coveralls to a specific file:
```shell
php-coveralls --json_path {{path/to/coveralls-upload.json}}
```
{% endraw %}