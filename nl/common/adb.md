---
layout: default
title: "adb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb">
  <a href="/nl/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug-Brug: communiceer met een Android-emulator of een aangesloten Android-apparaat.
> Meer informatie: <https://developer.android.com/studio/command-line/adb>.

#### Controleer of het adb serverproces draait en start het:
```shell
adb start-server
```
#### Sluit het adb serverproces:
```shell
adb kill-server
```
#### Start een afstandshell voor de doelemulator of apparaatinstantie:
```shell
adb shell
```
#### Stuur een Android-applicatie naar de emulator/het apparaat:
```shell
adb install -r {{pad/naar/bestand.apk}}
```
#### Kopiëer een bestand/map van het doelapparaat:
```shell
adb pull {{pad/naar/extern/bestand_of_map}} {{pad/naar/lokaal/bestand_of_map}}
```
#### Kopiëer een bestand/map naar het doelapparaat:
```shell
adb push {{pad/naar/lokaal/bestand_of_map}} {{pad/naar/extern/bestand_of_map}}
```
#### Krijg een lijst met aangesloten apparaten:
```shell
adb devices
```
{% endraw %}