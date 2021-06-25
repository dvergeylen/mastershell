---
layout: default
title: "pt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pt">
  <a href="/en/common/pt.html">pt</a> <a href="#pt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Platinum Searcher.
> A code search tool similar to `ag`.
> More information: <https://github.com/monochromegane/the_platinum_searcher>.

#### Find files containing "foo" and print the files with highlighted matches:
```shell
pt {{foo}}
```
#### Find files containing "foo" and display count of matches in each file:
```shell
pt -c {{foo}}
```
#### Find files containing "foo" as a whole word and ignore its case:
```shell
pt -wi {{foo}}
```
#### Find "foo" in files with a given extension using a regular expression:
```shell
pt -G='{{\.bar$}}' {{foo}}
```
#### Find files whose contents match the regular expression, up to 2 directories deep:
```shell
pt --depth={{2}} -e '{{^ba[rz]*$}}'
```
{% endraw %}