---
layout: default
title: "mytop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mytop">
  <a href="/en/common/mytop.html">mytop</a> <a href="#mytop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display MySQL server performance info like `top`.
> More information: <http://www.mysqlfanboy.com/mytop-3>.

#### Start mytop:
```shell
mytop
```
#### Connect with a specified username and password:
```shell
mytop -u {{user}} -p {{password}}
```
#### Connect with a specified username (the user will be prompted for a password):
```shell
mytop -u {{user}} --prompt
```
#### Do not show any idle (sleeping) threads:
```shell
mytop -u {{user}} -p {{password}} --noidle
```
{% endraw %}