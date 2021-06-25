---
layout: default
title: "aapt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aapt">
  <a href="/de/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Asset Packaging Tool.
> Kompiliere und verpacke die Resourcen einer Android App.
> Weitere Informationen: <https://elinux.org/Android_aapt>.

#### Liste alle Dateien eines APK Archivs auf:
```shell
aapt list {{pfad/zu/app.apk}}
```
#### Zeige die Metadaten einer App an (Version, Berechtigungen, usw.):
```shell
aapt dump badging {{pfad/zu/app.apk}}
```
#### Erstelle ein neues APK Archiv mit den Dateien eines bestimmten Verzeichnisses:
```shell
aapt package -F {{pfad/zu/app.apk}} {{pfad/zu/verzeichnis}}
```
{% endraw %}