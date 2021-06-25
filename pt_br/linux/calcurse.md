---
layout: default
title: "calcurse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="calcurse">
  <a href="/pt_br/linux/calcurse.html">calcurse</a> <a href="#calcurse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um calendário e agenda baseados em texto para a linha de comando.
> Mais informações: <https://calcurse.org>.

#### Iniciar o calcurse em modo interativo:
```shell
calcurse
```
#### Mostrar os agendamentos e eventos para o presente dia:
```shell
calcurse --appointment
```
#### Apagar todos os objetos gravados localmente e importar os objetos remotos:
```shell
calcurse-caldav --init=keep-remote
```
#### Apagar todos os objetos remotos e enviar os objetos gravados localmente:
```shell
calcurse-caldav --init=keep-local
```
#### Copiar os objetos gravados localmente para o servidor CalDAV e vice-versa:
```shell
calcurse-caldav --init=two-way
```
{% endraw %}