---
layout: default
title: "pidof"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pidof">
  <a href="/en/linux/pidof.html">pidof</a> <a href="#pidof"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gets the ID of a process using its name.

#### List all process IDs with given name:
```shell
pidof {{bash}}
```
#### List a single process ID with given name:
```shell
pidof -s {{bash}}
```
#### List process IDs including scripts with given name:
```shell
pidof -x {{script.py}}
```
#### Kill all processes with given name:
```shell
kill "$(pidof {{name}})" 
```
{% endraw %}