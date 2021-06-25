---
layout: default
title: "z"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="z">
  <a href="/en/common/z.html">z</a> <a href="#z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tracks the most used (by frecency) directories and enables quickly navigating to them using string patterns or regular expressions.
> More information: <https://github.com/rupa/z>.

#### Go to a directory that contains "foo" in the name:
```shell
z {{foo}}
```
#### Go to a directory that contains "foo" and then "bar":
```shell
z {{foo}} {{bar}}
```
#### Go to the highest-ranked directory matching "foo":
```shell
z -r {{foo}}
```
#### Go to the most recently accessed directory matching "foo":
```shell
z -t {{foo}}
```
#### List all directories in `z`'s database matching "foo":
```shell
z -l {{foo}}
```
#### Remove the current directory from `z`'s database:
```shell
z -x .
```
#### Restrict matches to subdirectories of the current directory:
```shell
z -c {{foo}}
```
{% endraw %}