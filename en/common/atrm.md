---
layout: default
title: "atrm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atrm">
  <a href="/en/common/atrm.html">atrm</a> <a href="#atrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove jobs scheduled by `at` or `batch` commands.
> To find job numbers use `atq`.
> More information: <https://man.archlinux.org/man/at.1>.

#### Remove job number 10:
```shell
atrm {{10}}
```
#### Remove many jobs, separated by spaces:
```shell
atrm {{15}} {{17}} {{22}}
```
{% endraw %}