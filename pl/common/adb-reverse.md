---
layout: default
title: "adb reverse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-reverse">
  <a href="/pl/common/adb-reverse.html">adb reverse</a> <a href="#adb-reverse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Reverse: zwrotne połączenie socketowe z emulowanego lub prawdziwego urządzenia Android.
> Więcej informacji: <https://developer.android.com/studio/command-line/adb>.

#### Listuj wszystkie zwrotne połączenia socketowe z emulatorów i urządzeń:
```shell
adb reverse --list
```
#### Przekieruj port TCP z emulatora lub urządzenia do localhost:
```shell
adb reverse tcp:{{remote_port}} tcp:{{local_port}}
```
#### Usuń wybrane zwrotne połączenie z emulatora lub urządzenia:
```shell
adb reverse --remove tcp:{{remote_port}}
```
#### Usuń wszystkie zwrotne połączenie z emulatorów lub urządzeń:
```shell
adb reverse --remove-all
```
{% endraw %}