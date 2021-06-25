---
layout: default
title: "man"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="man">
  <a href="/pt_br/common/man.html">man</a> <a href="#man"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para exibir páginas do manual.
> Mais informações: <https://www.man7.org/linux/man-pages/man1/man.1.html>.

#### Visualizar o manual de um comando:
```shell
man {{comando}}
```
#### Visualizar a página da seção 7 do manual de um comando:
```shell
man {{comando}}.{{7}}
```
#### Visualizar o caminho procurado pelas páginas do manual:
```shell
man --path
```
#### Visualizar o caminho do manual de um comando:
```shell
man -w {{comando}}
```
#### Procurar manuais contendo um termo de pesquisa:
```shell
man -k "{{termo_de_pesquisa}}"
```
{% endraw %}