---
layout: default
title: "wm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wm">
  <a href="/en/android/wm.html">wm</a> <a href="#wm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show information about the screen of an Android device.
> This command can only be used through `adb shell`.
> More information: <https://adbinstaller.com/commands/adb-shell-wm-5b672b17e7958178a2955538>.

#### Display the physical size of an Android device's screen:
```shell
wm {{size}}
```
#### Display the physical density of an Android device's screen:
```shell
wm {{density}}
```
{% endraw %}