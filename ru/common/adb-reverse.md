---
layout: default
title: "adb reverse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-reverse">
  <a href="/ru/common/adb-reverse.html">adb reverse</a> <a href="#adb-reverse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Reverse: обратное соединение от эмулятора Android или подключенного устройства Android.
> Больше информации: <https://developer.android.com/studio/command-line/adb>.

#### Вывести список всех обратных соединений от эмуляторов и устройств:
```shell
adb reverse --list
```
#### Создать обратное соединение по TCP-порту от эмулятора или устройства до localhost:
```shell
adb reverse tcp:{{удалённый_порт}} tcp:{{локальный_порт}}
```
#### Удалить обратное соединение из эмулятора или устройства:
```shell
adb reverse --remove tcp:{{удалённый_порт}}
```
#### Удалить все обратные соединения на всех эмуляторах и устройствах:
```shell
adb reverse --remove-all
```
{% endraw %}