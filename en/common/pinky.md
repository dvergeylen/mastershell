---
layout: default
title: "pinky"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pinky">
  <a href="/en/common/pinky.html">pinky</a> <a href="#pinky"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print user information using the `finger` protocol.

#### Display details about the current user:
```shell
pinky
```
#### Display details for a specific user:
```shell
pinky {{user}}
```
#### Display details in the long format:
```shell
pinky {{user}} -l
```
#### Omit the user's home directory and shell in long format:
```shell
pinky {{user}} -lb
```
#### Omit the user's project file in long format:
```shell
pinky {{user}} -lh
```
#### Omit the column headings in short format:
```shell
pinky {{user}} -f
```
{% endraw %}