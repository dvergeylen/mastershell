---
layout: default
title: "emacs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="emacs">
  <a href="/de/common/emacs.html">emacs</a> <a href="#emacs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Der erweiterbare, veränderbare und selbst-dokumentierende Echtzeit Text Editor.
> Siehe auch `emacsclient`.
> Weitere Informationen: <https://www.gnu.org/software/emacs>.

#### Öffne eine Datei in Emacs:
```shell
emacs {{pfad/zu/datei}}
```
#### Öffne eine Datei in einer bestimmten Zeile:
```shell
emacs +{{zeilennummer}} {{pfad/zu/datei}}
```
#### Starte Emacs in der Konsole (ohne X-Fenster):
```shell
emacs --no-window-system
```
#### Starte einen Emacs-Server im Hintergrund (aufrufbar mit `emacsclient`):
```shell
emacs --daemon
```
#### Beende einen laufenden Emacs-Server und alle Instanzen und frage nach Bestätigung für ungespeicherte Dateien:
```shell
emacsclient --eval '(save-buffers-kill-emacs)'
```
#### Tastenkombination zum Speichern einer Datei:
```shell
Ctrl + X, Ctrl + S
```
#### Tastenkombination zum Beenden von Emacs:
```shell
Ctrl + X, Ctrl + C
```
{% endraw %}