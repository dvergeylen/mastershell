---
layout: default
title: "mount"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mount">
  <a href="/it/common/mount.html">mount</a> <a href="#mount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fornisce accesso a un intero filesystem in una cartella specifica.

#### Mostra tutti i filesystem montati:
```shell
mount
```
#### Monta un dispositivo in una cartella:
```shell
mount -t {{tipo_di_filesystem}} {{percorso/al/dispositivo}} {{percorso/alla/cartella_desiderata}}
```
#### Monta un CD-ROM (con il filetypo ISO9660) a `/cdrom` (sola lettura):
```shell
mount -t {{iso9660}} -o ro {{/dev/cdrom}} {{/cdrom}}
```
#### Monta tutti i filesystem definiti in `/etc/fstab`:
```shell
mount -a
```
#### Monta un filesystem specifico descritto in `/etc/fstab` (ad esempio `/dev/sda1 /my_drive ext2 defaults 0 2`):
```shell
mount {{/my_drive}}
```
#### Monta una cartella in un'altra cartella:
```shell
mount --bind {{percorso/alla/vecchia_cartella}} {{percorso/alla/nuova_cartella}}
```
{% endraw %}