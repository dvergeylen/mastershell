---
layout: default
title: "aapt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aapt">
  <a href="/en/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Asset Packaging Tool.
> Compile and package an Android app's resources.
> More information: <https://elinux.org/Android_aapt>.

#### List files contained in an APK archive:
```shell
aapt list {{path/to/app.apk}}
```
#### Display an app's metadata (version, permissions, etc.):
```shell
aapt dump badging {{path/to/app.apk}}
```
#### Create a new APK archive with files from the specified directory:
```shell
aapt package -F {{path/to/app.apk}} {{path/to/directory}}
```
{% endraw %}