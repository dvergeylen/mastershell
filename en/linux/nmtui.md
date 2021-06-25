---
layout: default
title: "nmtui"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nmtui">
  <a href="/en/linux/nmtui.html">nmtui</a> <a href="#nmtui"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Text user interface for controlling NetworkManager.
> Use arrow keys to navigate, enter to select an option.

#### Open the user interface:
```shell
nmtui
```
#### Show a list of available connections, with the option to activate or deactivate them:
```shell
nmtui connect
```
#### Connect to a given network:
```shell
nmtui connect {{name|uuid|device|SSID}}
```
#### Edit/Add/Delete a given network:
```shell
nmtui edit {{name|id}}
```
#### Set the system hostname:
```shell
nmtui hostname
```
{% endraw %}