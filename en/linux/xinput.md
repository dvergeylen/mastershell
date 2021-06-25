---
layout: default
title: "xinput"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xinput">
  <a href="/en/linux/xinput.html">xinput</a> <a href="#xinput"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List available input devices, query information about a device and change input device settings.

#### List all input devices:
```shell
xinput list
```
#### Disable an input:
```shell
xinput disable {{id}}
```
#### Enable an input:
```shell
xinput enable {{id}}
```
#### Disconnect an input from its master:
```shell
xinput float {{id}}
```
#### Reattach an input as slave to a master:
```shell
xinput reattach {{id}} {{master_id}}
```
{% endraw %}