---
layout: default
title: "mandb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mandb">
  <a href="/en/linux/mandb.html">mandb</a> <a href="#mandb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the pre-formatted manual page database.
> More information: <https://man7.org/linux/man-pages/man8/mandb.8.html>.

#### Purge and process manual pages:
```shell
mandb
```
#### Update a single entry:
```shell
mandb --filename {{path/to/file}}
```
#### Create entries from scratch instead of updating:
```shell
mandb --create
```
#### Only process user databases:
```shell
mandb --user-db
```
#### Do not purge obsolete entries:
```shell
mandb --no-purge
```
#### Check the validity of manual pages:
```shell
mandb --test
```
{% endraw %}