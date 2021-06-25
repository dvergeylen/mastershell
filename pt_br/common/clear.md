---
layout: default
title: "clear"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clear">
  <a href="/pt_br/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Limpa a tela do terminal.
> Mais informações: <https://manned.org/clear>.

#### Limpar a tela (equivalente a apertar Control-L no terminal Bash):
```shell
clear
```
#### Limpar a tela mantendo o buffer de rolagem do terminal:
```shell
clear -x
```
#### Especificar o tipo de terminal a ser limpado (por padrão é o valor da variável de ambiente `TERM`):
```shell
clear -T {{tipo_do_terminal}}
```
#### Mostra a versão do `ncurses` usado pelo `clear`:
```shell
clear -V
```
{% endraw %}