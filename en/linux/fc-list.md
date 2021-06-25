---
layout: default
title: "fc-list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fc-list">
  <a href="/en/linux/fc-list.html">fc-list</a> <a href="#fc-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List available fonts installed on the system.

#### Return a list of installed fonts in your system:
```shell
fc-list
```
#### Return a list of installed fonts with given name:
```shell
fc-list | grep '{{DejaVu Serif}}'
```
#### Return the number of installed fonts in your system:
```shell
fc-list | wc -l
```
{% endraw %}