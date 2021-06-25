---
layout: default
title: "beep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="beep">
  <a href="/en/linux/beep.html">beep</a> <a href="#beep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A utility to beep the PC speaker.

#### Play a beep:
```shell
beep
```
#### Play a beep that repeats:
```shell
beep -r {{repetitions}}
```
#### Play a beep at a specified frequency (Hz) and duration (milliseconds):
```shell
beep -f {{frequency}} -l {{duration}}
```
#### Play each new frequency and duration as a distinct beep:
```shell
beep -f {{frequency}} -l {{duration}} -n -f {{frequency}} -l {{duration}}
```
#### Play the C major scale:
```shell
beep -f 262 -n -f 294 -n -f 330 -n -f 349 -n -f 392 -n -f 440 -n -f 494 -n -f 523
```
{% endraw %}