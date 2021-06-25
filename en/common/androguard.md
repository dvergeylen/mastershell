---
layout: default
title: "androguard"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="androguard">
  <a href="/en/common/androguard.html">androguard</a> <a href="#androguard"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reverse engineering tool for Android applications. Written in Python.
> More information: <https://github.com/androguard/androguard>.

#### Display Android app manifest:
```shell
androguard axml {{path/to/app.apk}}
```
#### Display app metadata (version and app ID):
```shell
androguard apkid {{path/to/app.apk}}
```
#### Decompile Java code from an app:
```shell
androguard decompile {{path/to/app.apk}} --output {{path/to/directory}}
```
{% endraw %}