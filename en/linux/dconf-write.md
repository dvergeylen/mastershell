---
layout: default
title: "dconf write"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dconf-write">
  <a href="/en/linux/dconf-write.html">dconf write</a> <a href="#dconf-write"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write a value to a dconf database path.
> More information: <https://developer.gnome.org/dconf>.

#### Write a string to a dconf path (note the nested quotes):
```shell
dconf write {{/example/dconf/path}} "'{{Example Value}}'"
```
#### Write a boolean to a dconf path:
```shell
dconf write {{/example/dconf/path}} {{true|false}}
```
#### Write an integer to a dconf path:
```shell
dconf write {{/example/dconf/path}} {{16}}
```
#### Write an array to a dconf path:
```shell
dconf write {{/example/dconf/path}} "[{{'My First Value', 'My Second Value'}}]"
```
#### Write an empty array to a dconf path:
```shell
dconf write {{/example/dconf/path}} "@as []"
```
{% endraw %}