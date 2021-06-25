---
layout: default
title: "lolcat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lolcat">
  <a href="/de/common/lolcat.html">lolcat</a> <a href="#lolcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Färbe Text in Regenbogenfarben ein.
> Weitere Informationen: <https://github.com/busyloop/lolcat>.

#### Gib den Inhalt einer Datei in Regenbogenfarben in der Konsole aus:
```shell
lolcat {{pfad/zu/datei}}
```
#### Gib die Ausgabe eines Befehls in Regenbogenfarben in der Konsole aus:
```shell
{{fortune}} | lolcat
```
#### Gib den Inhalt einer Datei in animierten Regenbogenfarben in der Konsole aus:
```shell
lolcat -a {{pfad/zu/datei}}
```
#### Gib den Inhalt einer Datei in 24-bit (truecolor) Regenbogenfarben in der Konsole aus:
```shell
lolcat -t {{pfad/zu/datei}}
```
{% endraw %}