---
layout: default
title: "adb install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-install">
  <a href="/it/common/adb-install.html">adb install</a> <a href="#adb-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Install: Invia pacchetti ad un emulatore Android od ad un dispositivo Android connesso.
> Maggiori informazioni: <https://developer.android.com/studio/command-line/adb>.

#### Invia un'applicazione Android ad un emulatore emulatore/Android:
```shell
adb install {{percorso/al/file.apk}}
```
#### Reinstalla una applicazione esistente, preservandone i dati:
```shell
adb install -r {{percorso/al/file.apk}}
```
#### Fornisce tutti i permessi elencati nel manifest dell'applicazione:
```shell
adb install -g {{percorso/al/file.apk}}
```
#### Aggiorna rapidamente un pacchetto installato aggiornando solamente le parti dell'APK che sono cambiate:
```shell
adb install --fastdeploy {{percorso/al/file.apk}}
```
{% endraw %}