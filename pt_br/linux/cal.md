---
layout: default
title: "cal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cal">
  <a href="/pt_br/linux/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe as informações do calendário, destacando o dia atual.

#### Exibir o calendário do mês atual:
```shell
cal
```
#### Exibir o calendário do meses anterior, atual e seguinte:
```shell
cal -3
```
#### Utilizar segunda-feira como o primeiro dia da semana:
```shell
cal --monday
```
#### Exibir o calendário de um ano específico (4 dígitos):
```shell
cal {{ano}}
```
#### Exibir o calendário para um mês e ano específico:
```shell
cal {{mes}} {{ano}}
```
{% endraw %}