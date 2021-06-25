---
layout: default
title: "fastboot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fastboot">
  <a href="/it/common/fastboot.html">fastboot</a> <a href="#fastboot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Comunica con il dispositivo Android connessione quando in modalità bootloader (la situazione in cui `adb` non funziona).
> Maggiori informazioni: <https://android.googlesource.com/platform/system/core/+/master/fastboot/#fastboot>.

#### Sblocca il bootloader:
```shell
fastboot oem unlock
```
#### Ri-blocca il bootloader:
```shell
fastboot oem lock
```
#### Riavvia il dispositivo da modalità fastboot, nuovamente in modalità fastboot:
```shell
fastboot reboot bootloader
```
#### Esegue in Flash di una data immagine:
```shell
fastboot flash {{file.zip}}
```
#### Esegue il Flash di una recovery image personalizzata:
```shell
fastboot flash recovery {{file.img}}
```
#### Mostra i dispositivi connessi:
```shell
fastboot devices
```
#### Mostra tutte le informazioni su un dispositivo:
```shell
fastboot getvar all
```
{% endraw %}