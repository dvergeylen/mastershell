---
layout: default
title: "doxygen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="doxygen">
  <a href="/pt_br/common/doxygen.html">doxygen</a> <a href="#doxygen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um sistema de documentação para várias linguagens de programação.
> Mais informações: <http://www.doxygen.nl>.

#### Gerar um arquivo de configuração padrão (Doxyfile):
```shell
doxygen -g
```
#### Gerar um arquivo de configuração, especificando o nome do arquivo de configuração:
```shell
doxygen -g {{caminho/para/arquivo_configuração}}
```
#### Gerar documentação utilizando um arquivo de configuração existente:
```shell
doxygen {{caminho/para/arquivo_configuração}}
```
{% endraw %}