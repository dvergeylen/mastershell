---
layout: default
title: "bison"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bison">
  <a href="/en/common/bison.html">bison</a> <a href="#bison"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU parser generator.
> More information: <https://www.gnu.org/software/bison/>.

#### Compile a bison definition file:
```shell
bison {{path/to/file.y}}
```
#### Compile in debug mode, which causes the resulting parser to write additional information to the standard output:
```shell
bison --debug {{path/to/file.y}}
```
#### Specify the output filename:
```shell
bison --output {{path/to/output.c}} {{path/to/file.y}}
```
#### Be verbose when compiling:
```shell
bison --verbose
```
{% endraw %}