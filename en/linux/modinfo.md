---
layout: default
title: "modinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="modinfo">
  <a href="/en/linux/modinfo.html">modinfo</a> <a href="#modinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract information about a Linux kernel module.

#### List all attributes of a kernel module:
```shell
modinfo {{kernel_module}}
```
#### List the specified attribute only:
```shell
modinfo -F {{author|description|license|parm|filename}} {{kernel_module}}
```
{% endraw %}