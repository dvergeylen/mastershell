---
layout: default
title: "adb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb">
  <a href="/pl/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: komunikuj się z instancją emulatora Androida lub podłączonym urządzeniem z Androidem.
> Więcej informacji: <https://developer.android.com/studio/command-line/adb>.

#### Sprawdź czy proces serwera adb działa, jeśli nie, uruchom go:
```shell
adb start-server
```
#### Zakończ proces serwera adb:
```shell
adb kill-server
```
#### Uruchom powłokę w instancji emulatora lub urządzeniu:
```shell
adb shell
```
#### Wypchnij aplikację Androidową do instancji emulatora lub urządzenia:
```shell
adb install -r {{ścieżka/do/pliku.apk}}
```
#### Skopiuj plik/katalog do urządzenia:
```shell
adb pull {{ścieżka/do/pliku_lub_katalogu_na_urządzeniu}} {{ścieżka/do/lokalnego_katalogu}}
```
#### Skopiuj plik/katalog z urządzenia:
```shell
adb push {{ścieżka/do/pliku_lub_katalogu_na_urządzeniu}} {{ścieżka/do/lokalnego_katalogu}}
```
#### Listuj połączone lub emulowane urządzenia:
```shell
adb devices
```
{% endraw %}