---
layout: default
title: "mat2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mat2">
  <a href="/en/common/mat2.html">mat2</a> <a href="#mat2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Anonymise various file formats by removing metadata.
> More information: <https://0xacab.org/jvoisin/mat2>.

#### List supported file formats:
```shell
mat2 --list
```
#### Remove metadata from a file:
```shell
mat2 {{path/to/file}}
```
#### Remove metadata from a file and print detailed output to the console:
```shell
mat2 --verbose {{path/to/file}}
```
#### Show metadata in a file without removing it:
```shell
mat2 --show {{path/to/file}}
```
#### Partially remove metadata from a file:
```shell
mat2 --lightweight {{path/to/file}}
```
{% endraw %}