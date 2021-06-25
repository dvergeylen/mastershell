---
layout: default
title: "pio update"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-update">
  <a href="/en/common/pio-update.html">pio update</a> <a href="#pio-update"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Update installed PlatformIO Core packages, development platforms and global libraries.
> See also: `pio platform update`, `pio lib update`.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_update.html>.

#### Perform a full update of all packages, development platforms and global libraries:
```shell
pio update
```
#### Update core packages only (skips platforms and libraries):
```shell
pio update --core-packages
```
#### Check for new versions of packages, platforms and libraries but do not actually update them:
```shell
pio update --dry-run
```
{% endraw %}