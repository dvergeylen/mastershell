---
layout: default
title: "jest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jest">
  <a href="/en/common/jest.html">jest</a> <a href="#jest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A zero-configuration JavaScript testing platform.
> More information: <https://jestjs.io>.

#### Run all available tests:
```shell
jest
```
#### Run the test suites from the given files:
```shell
jest {{path/to/file1}} {{path/to/file2}}
```
#### Run the test suites from files within the current and subdirectories, whose paths match the given regular expression:
```shell
jest {{regular_expression1}} {{regular_expression2}}
```
#### Run the tests whose names match the given regular expression:
```shell
jest --testNamePattern {{regular_expression}}
```
#### Run test suites related to a given source file:
```shell
jest --findRelatedTests {{path/to/source_file.js}}
```
#### Run test suites related to all uncommitted files:
```shell
jest --onlyChanged
```
#### Watch files for changes and automatically re-run related tests:
```shell
jest --watch
```
#### Show help:
```shell
jest --help
```
{% endraw %}