---
layout: default
title: "beep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="beep">
  <a href="/pt_br/linux/beep.html">beep</a> <a href="#beep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário que permite o computador emitir sons.

#### Emitir um som:
```shell
beep
```
#### Emitir um som repetidamente:
```shell
beep -r {{repeticoes}}
```
#### Emitir um som em uma frequência (Hz) específica e com duração específica (milisegundos):
```shell
beep -f {{frequencia}} -l {{duracao}}
```
#### Emitir cada frequência e duração como um som diferente:
```shell
beep -f {{frequencia}} -l {{duracao}} -n -f {{frequencia}} -l {{duracao}}
```
#### Executar a escala de Dó maior:
```shell
beep -f 262 -n -f 294 -n -f 330 -n -f 349 -n -f 392 -n -f 440 -n -f 494 -n -f 523
```
{% endraw %}