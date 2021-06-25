---
layout: default
title: "history"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="history">
  <a href="/pt_pt/common/history.html">history</a> <a href="#history"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Histórico da linha de comandos.

#### Mostrar o histórico da linha de comandos por ordem cronológica:
```shell
history
```
#### Apagar o histórico da linha de comandos:
```shell
history -c
```
#### Mostrar o enésimo comando no histórico da linha de comandos:
```shell
history !{{n}}
```
#### Mostrar as entradas do histórico da linha de comandos que correspondem a uma expressão regular:
```shell
history | grep {{expressao_regular}}
```
{% endraw %}