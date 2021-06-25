---
layout: default
title: "adb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb">
  <a href="/ru/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: управление запущенным эмулятором Android или подключенным устройством Android.
> Больше информации: <https://developer.android.com/studio/command-line/adb>.

#### Проверить, запущен ли процесс сервера adb и запустить его:
```shell
adb start-server
```
#### Завершить процесс сервера adb:
```shell
adb kill-server
```
#### Запустить удалённую оболочку на целевом эмуляторе/устройстве:
```shell
adb shell
```
#### Установить приложение Android на эмуляторе/устройстве:
```shell
adb install -r {{путь/до/файла.apk}}
```
#### Скопировать файл/папку с целевого устройства:
```shell
adb pull {{путь/до/папки_или_файла_на_устройстве}} {{путь/до/локальной_папки}}
```
#### Скопировать файл/папку на целевое устройство:
```shell
adb push {{путь/до/локального_файла_или_папки}} {{путь/до/целевой_папки_на_устройстве}}
```
#### Вывести список подключенных устройств:
```shell
adb devices
```
{% endraw %}