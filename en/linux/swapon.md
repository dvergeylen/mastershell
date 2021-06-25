---
layout: default
title: "swapon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="swapon">
  <a href="/en/linux/swapon.html">swapon</a> <a href="#swapon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enables device or file for swapping.

#### Get swap information:
```shell
swapon -s
```
#### Enable a given swap partition:
```shell
swapon {{/dev/sdb7}}
```
#### Enable a given swap file:
```shell
swapon {{path/to/file}}
```
#### Enable all swap areas:
```shell
swapon -a
```
#### Enable swap by label of a device or file:
```shell
swapon -L {{swap1}}
```
{% endraw %}