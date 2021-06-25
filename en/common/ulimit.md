---
layout: default
title: "ulimit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ulimit">
  <a href="/en/common/ulimit.html">ulimit</a> <a href="#ulimit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get and set user limits.

#### Get the properties of all the user limits:
```shell
ulimit -a
```
#### Get hard limit for the number of simultaneously opened files:
```shell
ulimit -H -n
```
#### Get soft limit for the number of simultaneously opened files:
```shell
ulimit -S -n
```
#### Set max per-user process limit:
```shell
ulimit -u 30
```
{% endraw %}