---
layout: default
title: "swig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="swig">
  <a href="/en/common/swig.html">swig</a> <a href="#swig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate bindings between C / C++ code and various high level languages such as JavaScript, Python, C#, and more.
> It uses special .i or .swg files to generate the bindings (C/C++ with SWIG directives, then outputs a C/C++ file that contains all of the wrapper code needed to build an extension module.

#### Generate a binding between C++ and Python:
```shell
swig -c++ -python -o {{path/to/output_wrapper.cpp}} {{path/to/swig_file.i}}
```
#### Generate a binding between C++ and Go:
```shell
swig -go -cgo -intgosize 64 -c++ {{path/to/swig_file.i}}
```
#### Generate a binding between C and Java:
```shell
swig -java {{path/to/swig_file.i}}
```
#### Generate a binding between C and Ruby and prefix the Ruby module with {{foo::bar::}}:
```shell
swig -ruby -prefix "{{foo::bar::}}" {{path/to/swig_file.i}}
```
{% endraw %}