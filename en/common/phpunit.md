---
layout: default
title: "phpunit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpunit">
  <a href="/en/common/phpunit.html">phpunit</a> <a href="#phpunit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PHPUnit command-line test runner.
> More information: <https://phpunit.de>.

#### Run tests in the current directory. Note: Expects you to have a 'phpunit.xml':
```shell
phpunit
```
#### Run tests in a specific file:
```shell
phpunit {{path/to/TestFile.php}}
```
#### Run tests annotated with the given group:
```shell
phpunit --group {{name}}
```
#### Run tests and generate a coverage report in HTML:
```shell
phpunit --coverage-html {{directory}}
```
{% endraw %}