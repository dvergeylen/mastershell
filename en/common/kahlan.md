---
layout: default
title: "kahlan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kahlan">
  <a href="/en/common/kahlan.html">kahlan</a> <a href="#kahlan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A unit and Behaviour Driven Development test framework for PHP.
> More information: <https://kahlan.github.io>.

#### Run all specifications in the "spec" directory:
```shell
kahlan
```
#### Run specifications using a specific configuration file:
```shell
kahlan --config={{path/to/configuration_file}}
```
#### Run specifications and output using a reporter:
```shell
kahlan --reporter={{dot|bar|json|tap|verbose}}
```
#### Run specifications with code coverage (detail can be between 0 and 4):
```shell
kahlan --coverage={{detail_level}}
```
{% endraw %}