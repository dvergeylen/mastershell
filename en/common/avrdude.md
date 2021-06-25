---
layout: default
title: "avrdude"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="avrdude">
  <a href="/en/common/avrdude.html">avrdude</a> <a href="#avrdude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Driver program for Atmel AVR microcontrollers programming.
> More information: <https://www.nongnu.org/avrdude/>.

#### Read AVR microcontroller:
```shell
avrdude -p {{AVR_device}} -c {{programmer}} -U flash:r:{{file.hex}}:i
```
#### Write AVR microcontroller:
```shell
avrdude -p {{AVR_device}} -c {{programmer}} -U flash:w:{{file.hex}}
```
#### List available AVR devices:
```shell
avrdude -p \?
```
#### List available AVR programmers:
```shell
avrdude -c \?
```
{% endraw %}