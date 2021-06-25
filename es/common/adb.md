---
layout: default
title: "adb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb">
  <a href="/es/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: comunica con una instancia de un emulador Android o conecta dispositivos Android.
> Más información: <https://developer.android.com/studio/command-line/adb>.

#### Verifica si el proceso del servidor adb está ejecutandose y lo inicia:
```shell
adb start-server
```
#### Termina el proceso del servidor adb:
```shell
adb kill-server
```
#### Inicia una terminal remota en la instance del emulador/dispositivo de destino:
```shell
adb shell
```
#### Instala una aplicación Android a un emulador/dispositivo:
```shell
adb install -r {{ruta/al/archivo.apk}}
```
#### Copia un archivo/directorio desde el dispositivo de destino:
```shell
adb pull {{ruta/al/archivo_o_directorio_en_el_dispositivo}} {{ruta/al/directorio_de_destino_local}}
```
#### Copia un archivo/directorio al dispositivo de destino:
```shell
adb push {{ruta/al/archivo_o_directorio_local}} {{ruta/al/directorio_de_destino_en_el_dispositivo}}
```
#### Obtiene una lista de dispositivos conectados:
```shell
adb devices
```
{% endraw %}