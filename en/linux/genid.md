---
layout: default
title: "genid"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="genid">
  <a href="/en/linux/genid.html">genid</a> <a href="#genid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate IDs, such as snowflakes, UUIDs, and a new GAID.
> More information: <https://github.com/bleonard252/genid>.

#### Generate a UUIDv4:
```shell
genid uuid
```
#### Generate a UUIDv5 using a namespace UUID and a specific name:
```shell
genid uuidv5 {{{ce598faa-8dd0-49ee-8525-9e24fff71dca}}} {{name}}
```
#### Generate a Discord Snowflake, without a trailing newline (useful in shell scripts):
```shell
genid --script snowflake
```
#### Generate a Generic Anonymous ID with a specific "real ID":
```shell
genid gaid {{real_id}}
```
#### Generate a Snowflake with the epoch set to a specific date:
```shell
genid snowflake --epoch={{unix_epoch_time}}
```
{% endraw %}