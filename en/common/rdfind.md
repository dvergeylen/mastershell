---
layout: default
title: "rdfind"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rdfind">
  <a href="/en/common/rdfind.html">rdfind</a> <a href="#rdfind"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find files with duplicate content and get rid of them.
> More information: <https://rdfind.pauldreik.se>.

#### Identify all duplicates in a given directory and output a summary:
```shell
rdfind -dryrun true {{path/to/directory}}
```
#### Replace all duplicates with hardlinks:
```shell
rdfind -makehardlinks true {{path/to/directory}}
```
#### Replace all duplicates with symlinks/soft links:
```shell
rdfind -makesymlinks true {{path/to/directory}}
```
#### Delete all duplicates and do not ignore empty files:
```shell
rdfind -deleteduplicates true -ignoreempty false {{path/to/directory}}
```
{% endraw %}