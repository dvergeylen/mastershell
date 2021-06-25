---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/de/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kopiere Dateien und Verzeichnisse.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/cp>.

#### Kopiere eine Datei an einen anderen Ort:
```shell
cp {{pfad/zu/datei}} {{pfad/zu/kopie}}
```
#### Kopiere eine Datei an einen anderen Ort und behalte den Dateinamen:
```shell
cp {{pfad/zu/datei}} {{pfad/zu/zielverzeichnis}}
```
#### Kopiere ein Verzeichnis rekursiv (falls der Zielort bereits existiert, wird das Verzeichnis in das Zielverzeichnis kopiert):
```shell
cp -r {{pfad/zu/verzeichnis}} {{pfad/zu/zielverzeichnis}}
```
#### Kopiere ein Verzeichnis rekursiv und gib alle Dateien aus, während sie kopiert werden:
```shell
cp -vr {{pfad/zu/verzeichnis}} {{pfad/zu/zielverzeichnis}}
```
#### Kopiere alle Textdateien in einem Verzeichnis und warte auf eine Bestätigung, falls eine Datei überschrieben werden soll:
```shell
cp -i {{/pfad/zu/*.txt}} {{pfad/zu/zielverzeichnis}}
```
#### Folge symbolischen Links vor dem Kopieren:
```shell
cp -L {{link}} {{pfad/zu/zielverzeichnis}}
```
{% endraw %}