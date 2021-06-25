---
layout: default
title: "twm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="twm">
  <a href="/en/common/twm.html">twm</a> <a href="#twm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A window manager for the X Window system.
> More information: <https://gitlab.freedesktop.org/xorg/app/twm>.

#### Connect to the default X server:
```shell
twm
```
#### Connect to a specific X server:
```shell
twm -display {{display}}
```
#### Only manage the default screen:
```shell
twm -s
```
#### Use a specific startup file:
```shell
twm -f {{path/to/file}}
```
#### Enable verbose mode and print unexpected errors in X:
```shell
twm -v
```
{% endraw %}