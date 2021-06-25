---
layout: default
title: "mktemp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mktemp">
  <a href="/en/common/mktemp.html">mktemp</a> <a href="#mktemp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a temporary file or directory.
> More information: <https://www.gnu.org/software/autogen/mktemp.html>.

#### Create an empty temporary file and return the absolute path to it:
```shell
mktemp
```
#### Create a temporary directory and return the absolute path to it:
```shell
mktemp -d
```
#### Create a temporary file with a specified suffix:
```shell
mktemp --suffix "{{.txt}}"
```
{% endraw %}