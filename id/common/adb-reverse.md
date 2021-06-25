---
layout: default
title: "adb reverse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-reverse">
  <a href="/id/common/adb-reverse.html">adb reverse</a> <a href="#adb-reverse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Reverse: membalik koneksi socket dari emulator Android atau perangkat Android terhubung.
> Informasi lebih lanjut: <https://developer.android.com/studio/command-line/adb>.

#### Daftar semua koneksi socket terbalik dari emulator dan perangkat:
```shell
adb reverse --list
```
#### Membalik port TCP dari emulator/perangkat ke localhost:
```shell
adb reverse tcp:{{port_jarak_jauh}} tcp:{{port_lokal}}
```
#### Melepas koneksi socket terbalik dari emulator/perangkat:
```shell
adb reverse --remove tcp:{{port_jarak_jauh}}
```
#### Melepas semua koneksi socket terbalik dari semua emulator dan perangkat:
```shell
adb reverse --remove-all
```
{% endraw %}