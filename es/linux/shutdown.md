---
layout: default
title: "shutdown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shutdown">
  <a href="/es/linux/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Detiene, apaga o reinicia la máquina.

#### Detiene inmediatamente:
```shell
shutdown -H now
```
#### Apaga inmediatamente:
```shell
shutdown -h now
```
#### Reinicia inmediatamente:
```shell
shutdown -r now
```
#### Reinicia dentro de 5 minutos:
```shell
shutdown -r +{{5}} &
```
#### Apaga a la 1:00 PM (formato 24h):
```shell
shutdown -h 13:00
```
#### Cancela una operación de apagado/reinicio pendiente:
```shell
shutdown -c
```
{% endraw %}