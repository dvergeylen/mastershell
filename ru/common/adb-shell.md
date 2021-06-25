---
layout: default
title: "adb shell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-shell">
  <a href="/ru/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: Запуск удалённой командной оболочки на эмуляторе Android или подключенном устройстве Android.
> Больше информации: <https://developer.android.com/studio/command-line/adb>.

#### Запустить удалённую интерактивную оболочку на эмуляторе или устройстве:
```shell
adb shell
```
#### Получить все свойства от эмулятора или устройства:
```shell
adb shell getprop
```
#### Вернуть всем разрешениям значение по умолчанию:
```shell
adb shell pm reset-permissions
```
#### Отозвать опасные разрешения для приложения:
```shell
adb shell pm revoke {{пакет}} {{разрешения}}
```
#### Вызвать событие клавиши:
```shell
adb shell input keyevent {{код_клавиши}}
```
#### Очистить данные приложения на эмуляторе или устройстве:
```shell
adb shell pm clear {{пакет}}
```
#### Запустить activity на эмуляторе или устройстве:
```shell
adb shell am start -n {{пакет}}/{{активность}}
```
#### Запустить базовый activity на эмуляторе или устройстве:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}