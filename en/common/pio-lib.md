---
layout: default
title: "pio lib"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-lib">
  <a href="/en/common/pio-lib.html">pio lib</a> <a href="#pio-lib"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage PlatformIO libraries.
> More information: <https://docs.platformio.org/en/latest/core/userguide/lib/>.

#### List installed libraries:
```shell
pio lib list
```
#### List built-in libraries based on installed development platforms and their frameworks:
```shell
pio lib builtin
```
#### Search for existing libraries:
```shell
pio lib search {{keyword}}
```
#### Show details about a library:
```shell
pio lib show {{library}}
```
#### Install a library:
```shell
pio lib install {{library}}
```
#### Update installed libraries:
```shell
pio lib update
```
#### Uninstall a library:
```shell
pio lib uninstall {{library}}
```
#### Show PlatformIO library registry statistics:
```shell
pio lib stats
```
{% endraw %}