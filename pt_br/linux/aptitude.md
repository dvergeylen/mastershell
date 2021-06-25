---
layout: default
title: "aptitude"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aptitude">
  <a href="/pt_br/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes das distribuições baseadas em Debian.
> Mais informações: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### Atualizar a lista de pacotes disponíveis (recomenda-se executá-lo antes de outros comandos `aptitude`):
```shell
aptitude update
```
#### Instalar um novo pacote e suas dependências:
```shell
aptitude install {{nome_do_pacote}}
```
#### Buscar pacotes correspondentes ao critério de busca:
```shell
aptitude search {{criterio_de_busca}}
```
#### Remover um pacote e todos que dependam dele:
```shell
aptitude remove {{nome_do_pacote}}
```
#### Atualizar os pacotes instalados para as versões mais recentes:
```shell
aptitude upgrade
```
#### Atualizar os pacotes instalados (semelhante ao `upgrade`), porém removendo os obsoletos e instalando pacotes solicitados por novas dependências:
```shell
aptitude full-upgrade
```
{% endraw %}