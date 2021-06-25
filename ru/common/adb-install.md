---
layout: default
title: "adb install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-install">
  <a href="/ru/common/adb-install.html">adb install</a> <a href="#adb-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Install: Установка пакетов на эмулятор Android или подключенное устройство Android.
> Больше информации: <https://developer.android.com/studio/command-line/adb>.

#### Установить приложение Android на эмулятор/устройство:
```shell
adb install {{путь/до/файла.apk}}
```
#### Переустановить существующее приложение, оставив его данные:
```shell
adb install -r {{путь/до/файла.apk}}
```
#### Дать все разрешения, перечисленные в манифесте приложения:
```shell
adb install -g {{путь/до/файла.apk}}
```
#### Быстрое обновление установленного пакета путём обновления только тех частей APK, которые изменились:
```shell
adb install --fastdeploy {{путь/до/файла.apk}}
```
{% endraw %}