---
layout: default
title: "ctest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ctest">
  <a href="/en/common/ctest.html">ctest</a> <a href="#ctest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CMake test driver program.
> More information: <https://gitlab.kitware.com/cmake/community/wikis/doc/ctest/Testing-With-CTest>.

#### Run all tests defined in the CMake project, executing 4 jobs at a time in parallel:
```shell
ctest -j{{4}} --output-on-failure
```
#### Show a list of available tests:
```shell
ctest -N
```
#### Run a single test based on its name, or filter on a regular expression:
```shell
ctest --output-on-failure -R '^{{test_name}}$'
```
{% endraw %}