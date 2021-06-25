---
layout: default
title: "ag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ag">
  <a href="/en/common/ag.html">ag</a> <a href="#ag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Silver Searcher. Like ack, but aims to be faster.
> More information: <https://github.com/ggreer/the_silver_searcher>.

#### Find files containing "foo", and print the line matches in context:
```shell
ag {{foo}}
```
#### Find files containing "foo" in a specific directory:
```shell
ag {{foo}} {{path/to/directory}}
```
#### Find files containing "foo", but only list the filenames:
```shell
ag -l {{foo}}
```
#### Find files containing "FOO" case-insensitively, and print only the match, rather than the whole line:
```shell
ag -i -o {{FOO}}
```
#### Find "foo" in files with a name matching "bar":
```shell
ag {{foo}} -G {{bar}}
```
#### Find files whose contents match a regular expression:
```shell
ag '{{^ba(r|z)$}}'
```
#### Find files with a name matching "foo":
```shell
ag -g {{foo}}
```
{% endraw %}