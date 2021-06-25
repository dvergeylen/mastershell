---
layout: default
title: "pest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pest">
  <a href="/en/common/pest.html">pest</a> <a href="#pest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP testing framework with a focus on simplicity.
> More information: <https://pestphp.com>.

#### Initialise a standard Pest configuration in the current directory:
```shell
pest --init
```
#### Run tests in the current directory:
```shell
pest
```
#### Run tests annotated with the given group:
```shell
pest --group {{name}}
```
#### Run tests and print the coverage report to stdout:
```shell
pest --coverage
```
#### Run tests with coverage and fail if the coverage is less than the minimum percentage:
```shell
pest --coverage --min={{80}}
```
{% endraw %}