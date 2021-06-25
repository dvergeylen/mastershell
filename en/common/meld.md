---
layout: default
title: "meld"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="meld">
  <a href="/en/common/meld.html">meld</a> <a href="#meld"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Graphical diffing and merging tool.
> More information: <https://meldmerge.org/>.

#### Start meld:
```shell
meld
```
#### Compare 2 files:
```shell
meld {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare 2 directories:
```shell
meld {{path/to/directory_1}} {{path/to/directory_2}}
```
#### Compare 3 files:
```shell
meld {{path/to/file_1}} {{path/to/file_2}} {{path/to/file_3}}
```
#### Open a comparison as a new tab in a pre-existing meld instance:
```shell
meld --newtab {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare multiple sets of files:
```shell
meld --diff {{path/to/file_1}} {{path/to/file_2}} --diff {{path/to/file_3}} {{path/to/file_4}}
```
{% endraw %}