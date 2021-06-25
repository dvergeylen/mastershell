---
layout: default
title: "f3probe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="f3probe">
  <a href="/en/common/f3probe.html">f3probe</a> <a href="#f3probe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Probe a block device (e.g. a flash drive or a microSD card) for counterfeit flash memory.
> See also `f3read`, `f3write`, `f3fix`.
> More information: <https://github.com/AltraMayor/f3>.

#### Probe a block device:
```shell
sudo f3probe {{path/to/block_device}}
```
#### Use the minimum about of RAM possible:
```shell
sudo f3probe --min-memory {{path/to/block_device}}
```
#### Time disk operations:
```shell
sudo f3probe --time-ops {{path/to/block_device}}
```
{% endraw %}