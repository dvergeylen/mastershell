---
layout: default
title: "locate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="locate">
  <a href="/en/linux/locate.html">locate</a> <a href="#locate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find filenames quickly.

#### Look for pattern in the database. Note: the database is recomputed periodically (usually weekly or daily):
```shell
locate {{pattern}}
```
#### Look for a file by its exact filename (a pattern containing no globbing characters is interpreted as `*pattern*`):
```shell
locate */{{filename}}
```
#### Recompute the database. You need to do it if you want to find recently added files:
```shell
sudo updatedb
```
{% endraw %}