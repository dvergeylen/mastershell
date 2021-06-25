---
layout: default
title: "chown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chown">
  <a href="/de/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ändere den Besitzer und die Besitzergruppe von Dateien und Verzeichnissen.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/chown>.

#### Ändere den Besitzer einer Datei/eines Verzeichnisses:
```shell
chown {{benutzer}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Ändere den Besitzer und die Besitzergruppe einer Datei/eines Verzeichnisses:
```shell
chown {{benutzer}}:{{gruppe}} {{pfad/zu/datei_oder_verzeichnis}}
```
#### Ändere den Besitzer eines Verzeichnisses rekursiv:
```shell
chown -R {{benutzer}} {{pfad/zu/verzeichnis}}
```
#### Ändere den Besitzer eines symbolischen Links:
```shell
chown -h {{benutzer}} {{pfad/zu/symlink}}
```
#### Ändere den Besitzer einer Datei/eines Verzeichnisses, damit sie/es mit einer Referenzdatei übereinstimmt:
```shell
chown --reference={{pfad/zu/referenzdatei_oder_verzeichnis}} {{pfad/zu/datei_oder_verzeichnis}}
```
{% endraw %}