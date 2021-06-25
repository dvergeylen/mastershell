---
layout: default
title: "mocha"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mocha">
  <a href="/en/common/mocha.html">mocha</a> <a href="#mocha"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute Mocha JavaScript test runner.
> More information: <https://mochajs.org>.

#### Run tests with default configuration or as configured in `mocha.opts`:
```shell
mocha
```
#### Run tests contained at a specific location:
```shell
mocha {{directory/with/tests}}
```
#### Run tests that match a specific grep pattern:
```shell
mocha --grep {{regular_expression}}
```
#### Run tests on changes to JavaScript files in the current directory and once initially:
```shell
mocha --watch
```
#### Run tests with a specific reporter:
```shell
mocha --reporter {{reporter}}
```
{% endraw %}