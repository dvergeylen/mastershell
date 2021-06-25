---
layout: default
title: "apktool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apktool">
  <a href="/en/common/apktool.html">apktool</a> <a href="#apktool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reverse engineer APK files.
> More information: <https://ibotpeaches.github.io/Apktool/>.

#### Decode an APK file:
```shell
apktool d {{file.apk}}
```
#### Build an APK file from a directory:
```shell
apktool b {{path/to/directory}}
```
#### Install and store frameworks:
```shell
apktool if {{framework.apk}}
```
{% endraw %}