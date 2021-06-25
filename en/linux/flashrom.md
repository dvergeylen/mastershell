---
layout: default
title: "flashrom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flashrom">
  <a href="/en/linux/flashrom.html">flashrom</a> <a href="#flashrom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read, write, verify and erase flash chips.
> More information: <https://manned.org/flashrom>.

#### Probe the chip, ensuring the wiring is correct:
```shell
flashrom --programmer {{programmer}}
```
#### Read flash and save it to a file:
```shell
flashrom -p {{programmer}} --read {{path/to/file}}
```
#### Write a file to the flash:
```shell
flashrom -p {{programmer}} --write {{path/to/file}}
```
#### Verify the flash against a file:
```shell
flashrom -p {{programmer}} --verify {{path/to/file}}
```
#### Probe the chip using RaspberryPi:
```shell
flashrom -p {{linux_spi:dev=/dev/spidev0.0}}
```
{% endraw %}