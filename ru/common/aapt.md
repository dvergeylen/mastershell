---
layout: default
title: "aapt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aapt">
  <a href="/ru/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Утилита для упаковки ресурсов для Android.
> Компилирует и упаковывает ресурсы приложений Android.

#### Вывести список файлов содержащихся в APK-архиве:
```shell
aapt list {{путь/до/приложения.apk}}
```
#### Отобразить мета-данные приложения (версия, разрешения, и т.д.):
```shell
aapt dump badging {{путь/до/приложения.apk}}
```
#### Создать новый APK-архив с файлами из указанной папки:
```shell
aapt package -F {{путь/до/приложения.apk}} {{путь/до/папки}}
```
{% endraw %}