---
layout: default
title: "fakedata"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fakedata">
  <a href="/en/common/fakedata.html">fakedata</a> <a href="#fakedata"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate fake data using a large variety of generators.
> More information: <https://github.com/lucapette/fakedata>.

#### List all valid generators:
```shell
fakedata --generators
```
#### Generate data using one or more generators:
```shell
fakedata {{generator1}} {{generator2}}
```
#### Generate data with a specific output format:
```shell
fakedata --format {{csv|tab|sql}} {{generator}}
```
#### Generate a given number of data items (defaults to 10):
```shell
fakedata --limit {{n}} {{generator}}
```
#### Generate data using a custom output template (the first letter of generator names must be capitalized):
```shell
echo "{{\{\{Generator\}\}}}" | fakedata
```
{% endraw %}