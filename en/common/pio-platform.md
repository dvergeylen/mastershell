---
layout: default
title: "pio platform"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-platform">
  <a href="/en/common/pio-platform.html">pio platform</a> <a href="#pio-platform"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage PlatformIO development platforms.
> More information: <https://docs.platformio.org/en/latest/core/userguide/platforms/>.

#### List all installed development platforms:
```shell
pio platform list
```
#### Search for existing development platforms:
```shell
pio platform search {{platform}}
```
#### Show details about a development platform:
```shell
pio platform show {{platform}}
```
#### Install a development platform:
```shell
pio platform install {{platform}}
```
#### Update installed development platforms:
```shell
pio platfom update
```
#### Uninstall a development platform:
```shell
pio platform uninstall {{platform}}
```
#### List all supported frameworks:
```shell
pio platform frameworks
```
{% endraw %}