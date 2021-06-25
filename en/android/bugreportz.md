---
layout: default
title: "bugreportz"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bugreportz">
  <a href="/en/android/bugreportz.html">bugreportz</a> <a href="#bugreportz"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a zipped Android bug report.
> This command can only be used through `adb shell`.
> More information: <https://android.googlesource.com/platform/frameworks/native/+/master/cmds/bugreportz/>.

#### Generate a complete zipped bug report of an Android device:
```shell
bugreportz
```
#### Show the progress of a running `bugreportz` operation:
```shell
bugreportz -p
```
#### Show the version of `bugreportz`:
```shell
bugreportz -v
```
#### Display help:
```shell
bugreportz -h
```
{% endraw %}