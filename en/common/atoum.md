---
layout: default
title: "atoum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atoum">
  <a href="/en/common/atoum.html">atoum</a> <a href="#atoum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple, modern and intuitive unit testing framework for PHP.
> More information: <http://atoum.org>.

#### Initialise a configuration file:
```shell
atoum --init
```
#### Run all tests:
```shell
atoum
```
#### Run tests using the specified configuration file:
```shell
atoum -c {{path/to/file}}
```
#### Run a specific test file:
```shell
atoum -f {{path/to/file}}
```
#### Run a specific directory of tests:
```shell
atoum -d {{path/to/directory}}
```
#### Run all tests under a specific namespace:
```shell
atoum -ns {{namespace}}
```
#### Run all tests with a specific tag:
```shell
atoum -t {{tag}}
```
#### Load a custom bootstrap file before running tests:
```shell
atoum --bootstrap-file {{path/to/file}}
```
{% endraw %}