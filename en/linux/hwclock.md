---
layout: default
title: "hwclock"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hwclock">
  <a href="/en/linux/hwclock.html">hwclock</a> <a href="#hwclock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Used for reading or changing the hardware clock. Usually requires root.

#### Display the current time as reported by the hardware clock:
```shell
hwclock
```
#### Write the current software clock time to the hardware clock (sometimes used during system setup):
```shell
hwclock --systohc
```
#### Write the current hardware clock time to the software clock:
```shell
hwclock --hctosys
```
{% endraw %}