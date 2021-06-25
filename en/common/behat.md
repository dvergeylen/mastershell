---
layout: default
title: "behat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="behat">
  <a href="/en/common/behat.html">behat</a> <a href="#behat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP framework for Behaviour-Driven Development.
> More information: <https://behat.org>.

#### Initialise a new Behat project:
```shell
behat --init
```
#### Run all tests:
```shell
behat
```
#### Run all tests from the specified suite:
```shell
behat --suite={{suite_name}}
```
#### Run tests with a specific output formatter:
```shell
behat --format {{pretty|progress}}
```
#### Run tests and output results to a file:
```shell
behat --out {{path/to/file}}
```
#### Display a list of definitions in your test suites:
```shell
behat --definitions
```
{% endraw %}