---
layout: default
title: "pio system"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-system">
  <a href="/en/common/pio-system.html">pio system</a> <a href="#pio-system"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Miscellaneous system commands for PlatformIO.
> More information: <https://docs.platformio.org/en/latest/core/userguide/system/>.

#### Install shell completion for the current shell (supports bash, fish, zsh and powershell):
```shell
pio system completion install
```
#### Uninstall shell completion for the current shell:
```shell
pio system completion uninstall
```
#### Display system-wide PlatformIO information:
```shell
pio system info
```
#### Remove unused PlatformIO data:
```shell
pio system prune
```
#### Remove only cached data:
```shell
pio system prune --cache
```
#### List unused PlatformIO data that would be removed but do not actually remove it:
```shell
pio system prune --dry-run
```
{% endraw %}