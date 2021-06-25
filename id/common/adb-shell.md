---
layout: default
title: "adb shell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-shell">
  <a href="/id/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: Menjalankan perintah shell jarak jauh pada emulator Android atau perangkat Android terhubung.
> Informasi lebih lanjut: <https://developer.android.com/studio/command-line/adb>.

#### Memulai shell interaktif jarak jauh di emulator/perangkat:
```shell
adb shell
```
#### Mendapatkan semua properti dari emulator/perangkat:
```shell
adb shell getprop
```
#### Mengembalikan semua izin runtime ke default:
```shell
adb shell pm reset-permissions
```
#### Mencabut izin berbahaya dari sebuah aplikasi:
```shell
adb shell pm revoke {{paket}} {{izin}}
```
#### Memicu sebuah peristiwa penting:
```shell
adb shell input keyevent {{keycode}}
```
#### Mengosongkan data aplikasi pada emulator/perangkat:
```shell
adb shell pm clear {{paket}}
```
#### Memulai aktivitas pada emulator/perangkat:
```shell
adb shell am start -n {{paket}}/{{aktivitas}}
```
#### Memulai aktivitas beranda pada emulator/perangkat:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}