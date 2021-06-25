---
layout: default
title: "set"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="set">
  <a href="/en/common/set.html">set</a> <a href="#set"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display, set or unset values of shell attributes and positional parameters.

#### Display the names and values of shell variables:
```shell
set
```
#### Mark variables that are modified or created for export:
```shell
set -a
```
#### Notify of job termination immediately:
```shell
set -b
```
#### Set various options, e.g. enable `vi` style line editing:
```shell
set -o {{vi}}
```
{% endraw %}