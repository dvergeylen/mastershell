---
layout: default
title: "avrdude"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="avrdude">
  <a href="/de/common/avrdude.html">avrdude</a> <a href="#avrdude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Treiberprogramm für Atmel AVR Mikrocontroller-Programmierung.
> Weitere Informationen: <https://www.nongnu.org/avrdude/>.

#### Schreibt den Speicherinhalt eines AVR-Mikrocontrollers in eine Datei:
```shell
avrdude -p {{avr_gerät}} -c {{programmer}} -U flash:r:{{pfad/zu/datei.hex}}:i
```
#### Schreibt den Inhalt einer Datei in einen AVR-Mikrocontroller:
```shell
avrdude -p {{avr_gerät}} -c {{programmer}} -U flash:w:{{pfad/zu/datei.hex}}
```
#### Liste alle verfügbaren AVR-Geräte auf:
```shell
avrdude -p \?
```
#### Liste alle verfügbaren AVR-Programmer auf:
```shell
avrdude -c \?
```
{% endraw %}