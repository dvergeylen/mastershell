---
layout: default
title: "objdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="objdump">
  <a href="/en/common/objdump.html">objdump</a> <a href="#objdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View information about object files.

#### Display the file header information:
```shell
objdump -f {{binary}}
```
#### Display the dis-assembled output of executable sections:
```shell
objdump -d {{binary}}
```
#### Display a complete binary hex dump of all sections:
```shell
objdump -s {{binary}}
```
{% endraw %}