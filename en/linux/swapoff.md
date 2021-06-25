---
layout: default
title: "swapoff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="swapoff">
  <a href="/en/linux/swapoff.html">swapoff</a> <a href="#swapoff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disables device or file for swapping.

#### Disable a given swap partition:
```shell
swapoff {{/dev/sdb7}}
```
#### Disable a given swap file:
```shell
swapoff {{path/to/file}}
```
#### Disable all swap areas:
```shell
swapoff -a
```
#### Disable swap by label of a device or file:
```shell
swapoff -L {{swap1}}
```
{% endraw %}