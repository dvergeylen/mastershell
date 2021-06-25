---
layout: default
title: "adb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb">
  <a href="/it/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: comunica con un'instanza di un emulatore Android o con un dispositivo android connesso.
> Maggiori informazioni: <https://developer.android.com/studio/command-line/adb>.

#### Controlla se il processo server adb è attivo ed avvialo:
```shell
adb start-server
```
#### Termina il processo server adb:
```shell
adb kill-server
```
#### Avvia una shell remota nell'emulatore o dispositivo target:
```shell
adb shell
```
#### Installa un'applicazione Android nell'emulatore o dispositivo target:
```shell
adb install -r {{percorso/al/file.apk}}
```
#### Copia file o directory dal dispositivo target:
```shell
adb pull {{percorso/a/file_o_directory_dispositivo}} {{percorso/a/file_o_directory_locale}}
```
#### Copia file/directory sul dispositivo target:
```shell
adb push {{percorso/a/file_o_directory_locale}} {{percorso/a/directory_destinazione_dispositivo}}
```
#### Mostra una lista dei dispositivi connessi:
```shell
adb devices
```
{% endraw %}