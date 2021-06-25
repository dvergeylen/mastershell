---
layout: default
title: "ipcs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipcs">
  <a href="/en/common/ipcs.html">ipcs</a> <a href="#ipcs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about resources used in IPC (Inter-process Communication).

#### Specific information about the Message Queue which has the id 32768:
```shell
ipcs -qi 32768
```
#### General information about all the IPC:
```shell
ipcs -a
```
{% endraw %}