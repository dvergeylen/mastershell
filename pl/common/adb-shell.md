---
layout: default
title: "adb shell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-shell">
  <a href="/pl/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: uruchamiaj zdalne polecenia powłoki na instancji emulatora Androida lub podłączonych urządzeniach z Androidem.
> Więcej informacji: <https://developer.android.com/studio/command-line/adb>.

#### Uruchom interaktywną zdalną powłokę na emulatorze / urządzeniu:
```shell
adb shell
```
#### Pobierz wszystkie właściwości z emulatora lub urządzenia:
```shell
adb shell getprop
```
#### Przywróć wszystkie uprawnienia wykonawcze do ich wartości domyślnych:
```shell
adb shell pm reset-permissions
```
#### Odwołaj niebezpieczne pozwolenie dla aplikacji:
```shell
adb shell pm revoke {{paczka}} {{pozwolenie}}
```
#### Wywołaj zdarzenie klawisza:
```shell
adb shell input keyevent {{kod_klucza}}
```
#### Wyczyść dane aplikacji na emulatorze lub urządzeniu:
```shell
adb shell pm clear {{paczka}}
```
#### Rozpocznij aktywność na emulatorze / urządzeniu:
```shell
adb shell am start -n {{paczka}}/{{aktywność}}
```
#### Rozpocznij aktywność domową na emulatorze lub urządzeniu:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}