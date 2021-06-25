---
layout: default
title: "macchanger"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="macchanger">
  <a href="/en/linux/macchanger.html">macchanger</a> <a href="#macchanger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line utility for manipulating network interface MAC addresses.

#### View the current and permanent MAC addresses of a interface:
```shell
macchanger --show {{interface}}
```
#### Set interface to a random MAC:
```shell
macchanger --random {{interface}}
```
#### Set interface to a specific MAC:
```shell
macchanger --mac {{XX:XX:XX:XX:XX:XX}} {{interface}}
```
#### Reset interface to its permanent hardware MAC:
```shell
macchanger --permanent {{interface}}
```
{% endraw %}