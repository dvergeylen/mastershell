---
layout: default
title: "lebab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lebab">
  <a href="/en/common/lebab.html">lebab</a> <a href="#lebab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A JavaScript modernizer for transpiling code to ES6/ES7.
> Transformations must be provided for all examples.
> More information: <https://github.com/lebab/lebab>.

#### Display a list of the available transformations:
```shell
lebab --help
```
#### Transpile using one or more comma-separated transformations:
```shell
lebab --transform {{transformation}}
```
#### Transpile a file to stdout:
```shell
lebab {{path/to/input_file}}
```
#### Transpile a file to the specified output file:
```shell
lebab {{path/to/input_file}} --out-file {{path/to/output_file}}
```
#### Replace all `.js` files in-place in the specified directory, glob or file:
```shell
lebab --replace {{directory|glob|file}}
```
{% endraw %}