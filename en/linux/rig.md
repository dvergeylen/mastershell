---
layout: default
title: "rig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rig">
  <a href="/en/linux/rig.html">rig</a> <a href="#rig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to piece together a random first name, last name, street number and address, along with a geographically consistent (ie, they all match the same area) city, state, ZIP code, and area code.
> More information: <https://manpages.ubuntu.com/manpages/focal/man6/rig.6.html>.

#### Display a random name (male or female) and address:
```shell
rig
```
#### Display a [m]ale (or [f]emale) random name and address:
```shell
rig -{{m|f}}
```
#### Use data files from a specific directory (default is `/usr/share/rig`):
```shell
rig -d {{path/to/directory}}
```
#### Display a specific number of identities:
```shell
rig -c {{number}}
```
#### Display a specific number of female identities:
```shell
rig -f -c {{number}}
```
{% endraw %}