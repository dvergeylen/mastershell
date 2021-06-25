---
layout: default
title: "less"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="less">
  <a href="/de/common/less.html">less</a> <a href="#less"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Öffne eine Datei für interaktives lesen, erlaubt scrollen und suchen.

#### Öffne eine Datei:
```shell
less {{pfad/zu/datei}}
```
#### Scrolle eine Seite runter / hoch:
```shell
<Leertaste> (runter), b (hoch)
```
#### Springe zum Ende / Anfang der Datei:
```shell
G (Ende), g (Anfang)
```
#### Suche nach einer Zeichenkette forwärts (n/N um zur nächsten/vorherigen Übereinstimmung zu springen):
```shell
/{{suche}}
```
#### Suche nach einer Zeichenkette rückwärts (n/N um zur nächsten/vorherigen Übereinstimmung zu springen):
```shell
?{{suche}}
```
#### Folge der Ausgabe des geöffeten Buffers:
```shell
F
```
#### Öffne die Datei in einem Editor:
```shell
v
```
#### Beende `less`:
```shell
q
```
{% endraw %}