---
layout: default
title: "wall"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wall">
  <a href="/en/linux/wall.html">wall</a> <a href="#wall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write a message on the terminals of users currently logged in.

#### Send a message:
```shell
echo "{{message}}" | wall
```
#### Send a message from a file:
```shell
wall {{file}}
```
#### Send a message with timeout (default 300):
```shell
wall -t {{seconds}} {{file}}
```
{% endraw %}