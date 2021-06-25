---
layout: default
title: "pm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pm">
  <a href="/en/android/pm.html">pm</a> <a href="#pm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show information about apps on an Android device.
> More information: <https://developer.android.com/studio/command-line/adb#pm>.

#### Print a list of all installed apps:
```shell
pm list packages
```
#### Print a list of all installed system apps:
```shell
pm list packages -s
```
#### Print a list of all installed 3rd-Party apps:
```shell
pm list packages -3
```
#### Print a list of apps matching specific keywords:
```shell
pm list packages {{keywords}}
```
#### Print the path of the APK of a specific app:
```shell
pm path {{app}}
```
{% endraw %}