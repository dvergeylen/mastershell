---
layout: default
title: "bmon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bmon">
  <a href="/pt_br/linux/bmon.html">bmon</a> <a href="#bmon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitora a largura de banda e produz estatísticas relacionadas a rede.

#### Exibir uma lista com todas as interfaces de rede:
```shell
bmon -a
```
#### Exibir as taxas de transferência de dados em bits por segundo:
```shell
bmon -b
```
#### Definir quais interfaces serão visíveis:
```shell
bmon -p {{interface_1,interface_2,interface_3}}
```
#### Definir o intervalo (em segundos) que a taxa por contador será calculada:
```shell
bmon -R {{2.0}}
```
{% endraw %}