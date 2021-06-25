---
layout: default
title: "emacsclient"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="emacsclient">
  <a href="/de/common/emacsclient.html">emacsclient</a> <a href="#emacsclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Öffnet Dateien in einem laufenden Emacs-Server.
> Siehe auch `emacs`.
> Weitere Informationen: <https://www.emacswiki.org/emacs/EmacsClient>.

#### Öffne eine Datei in einem laufenden Emacs-Server (mit GUI wenn möglich):
```shell
emacsclient {{pfad/zu/datei}}
```
#### Öffne eine Datei in der Konsole (ohne X-Fenster):
```shell
emacsclient --no-window-system {{pfad/zu/datei}}
```
#### Öffne eine Datei in einem neuen Emacs Fenster:
```shell
emacsclient --create-frame {{pfad/zu/datei}}
```
#### Führe einen Befehl aus und schreibe das Ergebnis in stdout:
```shell
emacsclient --eval '({{befehl}})'
```
#### Gib einen alternativen Editor an für den Fall, dass kein Emacs-Server läuft:
```shell
emacsclient --alternate-editor {{editor}} {{pfad/zu/datei}}
```
#### Beende einen laufenden Emacs-Server und alle Instanzen und frage nach Bestätigung für ungespeicherte Dateien:
```shell
emacsclient --eval '(save-buffers-kill-emacs)'
```
{% endraw %}