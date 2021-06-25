---
layout: default
title: "strip-nondeterminism"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="strip-nondeterminism">
  <a href="/en/common/strip-nondeterminism.html">strip-nondeterminism</a> <a href="#strip-nondeterminism"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to remove non-deterministic information (e.g. timestamps) from files.
> More information: <https://salsa.debian.org/reproducible-builds/strip-nondeterminism>.

#### Strip nondeterministic information from a file:
```shell
strip-nondeterminism {{path/to/file}}
```
#### Strip nondeterministic information from a file manually specifying the filetype:
```shell
strip-nondeterminism --type {{filetype}} {{path/to/file}}
```
#### Strip nondeterministic information from a file; instead of removing timestamps set them to the specified UNIX timestamp:
```shell
strip-nondeterminism --timestamp {{unix_timestamp}} {{path/to/file}}
```
{% endraw %}