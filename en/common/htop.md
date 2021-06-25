---
layout: default
title: "htop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="htop">
  <a href="/en/common/htop.html">htop</a> <a href="#htop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dynamic real-time information about running processes. An enhanced version of `top`.

#### Start htop:
```shell
htop
```
#### Start htop displaying only processes owned by given user:
```shell
htop -u {{username}}
```
#### Sort processes by a column (use `--sort-key help` for a column list):
```shell
htop -s {{column_name}}
```
#### Get help about interactive commands:
```shell
?
```
{% endraw %}