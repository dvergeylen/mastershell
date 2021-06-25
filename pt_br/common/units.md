---
layout: default
title: "units"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="units">
  <a href="/pt_br/common/units.html">units</a> <a href="#units"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Realiza a conversão entre duas unidades de medida.
> Mais informações: <https://www.gnu.org/software/units/>.

#### Rodar no modo interativo:
```shell
units
```
#### Mostrar a conversão entre duas unidades simples:
```shell
units {{quarts}} {{tablespoons}}
```
#### Converter entre unidades com quantidades definidas:
```shell
units {{15 pounds}} {{kilograms}}
```
#### Mostrar a conversão entre duas unidades compostas:
```shell
units "{{meters / second}}" "{{inches / hour}}"
```
#### Mostrar a conversão entre unidades de diferentes dimensões:
```shell
units "{{acres}}" "{{ft^2}}"
```
{% endraw %}