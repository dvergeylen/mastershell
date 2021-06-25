---
layout: default
title: "mkfile"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfile">
  <a href="/en/osx/mkfile.html">mkfile</a> <a href="#mkfile"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create one or more empty files of any size.

#### Create an empty file of 15 kilobytes:
```shell
mkfile -n {{15k}} {{filename}}
```
#### Create a file of a given size and unit (bytes, KB, MB, GB):
```shell
mkfile -n {{size}}{{b|k|m|g}} {{filename}}
```
#### Create two files of 4 megabytes each:
```shell
mkfile -n {{4m}} {{first_filename}} {{second_filename}}
```
{% endraw %}