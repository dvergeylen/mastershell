---
layout: default
title: "avrdude"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="avrdude">
  <a href="/it/common/avrdude.html">avrdude</a> <a href="#avrdude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Driver per il programmatore di microcontrollori Atmel AVR.
> Maggiori informazioni: <https://www.nongnu.org/avrdude/>.

#### Leggi dal microcontrollore AVR:
```shell
avrdude -p {{dispositivo_AVR}} -c {{id_programmatore}} -U flash:r:{{file.hex}}:i
```
#### Scrivi sul microcontrollore AVR:
```shell
avrdude -p {{dispositivo_AVR}} -c {{id_programmatore}} -U flash:w:{{file.hex}}
```
#### Elenca dispositivi AVR disponibili:
```shell
avrdude -p \?
```
#### Elenca programmatori AVR disponibili:
```shell
avrdude -c \?
```
{% endraw %}