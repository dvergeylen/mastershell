---
layout: default
title: "inxi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="inxi">
  <a href="/en/linux/inxi.html">inxi</a> <a href="#inxi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print a summary of system information and resources for debugging purposes.

#### Print a short summary of CPU, memory, hard drive and kernel information:
```shell
inxi
```
#### Print a full description of CPU, memory, disk, network and process information:
```shell
inxi -Fz
```
#### Print information about the distribution's repository:
```shell
inxi -r
```
{% endraw %}