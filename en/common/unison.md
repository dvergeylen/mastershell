---
layout: default
title: "unison"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unison">
  <a href="/en/common/unison.html">unison</a> <a href="#unison"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bidirectional file synchronisation tool.
> More information: <https://www.cis.upenn.edu/~bcpierce/unison/download/releases/stable/unison-manual.html>.

#### Sync two directories (creates log first time these two directories are synchronised):
```shell
unison {{path/to/directory_1}} {{path/to/directory_2}}
```
#### Automatically accept the (non-conflicting) defaults:
```shell
unison {{path/to/directory_1}} {{path/to/directory_2}} -auto
```
#### Ignore some files using a pattern:
```shell
unison {{path/to/directory_1}} {{path/to/directory_2}} -ignore {{pattern}}
```
#### Show documentation:
```shell
unison -doc {{topics}}
```
{% endraw %}