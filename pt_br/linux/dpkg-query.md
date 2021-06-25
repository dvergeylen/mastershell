---
layout: default
title: "dpkg-query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dpkg-query">
  <a href="/pt_br/linux/dpkg-query.html">dpkg-query</a> <a href="#dpkg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta que mostra informações dos pacotes instalados.

#### Exibir os pacotes instalados:
```shell
dpkg-query -l
```
#### Exibir os pacotes instalados correspondentes ao critério de busca:
```shell
dpkg-query -l '{{criterio_de_busca}}'
```
#### Exibir todos os arquivos instalados por um pacote:
```shell
dpkg-query -L {{nome_do_pacote}}
```
#### Exibir informações sobre um pacote:
```shell
dpkg-query -s {{nome_do_pacote}}
```
{% endraw %}