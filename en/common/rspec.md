---
layout: default
title: "rspec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rspec">
  <a href="/en/common/rspec.html">rspec</a> <a href="#rspec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Behavior-driven development testing framework written in Ruby to test Ruby code.
> More information: <https://rspec.info>.

#### Initialise an .rspec config and a spec helper file:
```shell
rspec --init
```
#### Run all tests:
```shell
rspec
```
#### Run a specific directory of tests:
```shell
rspec {{path/to/directory}}
```
#### Run a specific test file:
```shell
rspec {{path/to/file}}
```
#### Run multiple test files:
```shell
rspec {{path/to/file1}} {{path/to/file2}}
```
#### Run a specific test in a file (e.g. the test starts on line 83):
```shell
rspec {{path/to/file}}:{{83}}
```
#### Run specs with a specific seed:
```shell
rspec --seed {{seed_number}}
```
{% endraw %}