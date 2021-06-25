---
layout: default
title: "apt-cache"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-cache">
  <a href="/pt_br/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Buscador de pacotes para distribuições baseadas no Debian.
> Mais informações: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Buscar pacotes, no cache de pacotes APT, correspondentes ao critério de busca:
```shell
apt-cache search {{criterio_de_busca}}
```
#### Exibir informações sobre um pacote:
```shell
apt-cache show {{nome_do_pacote}}
```
#### Informar a situação de um pacote, se ele está instalado e atualizado:
```shell
apt-cache policy {{nome_do_pacote}}
```
#### Exibir as dependências de um pacote:
```shell
apt-cache depends {{nome_do_pacote}}
```
#### Exibir pacotes dependentes de um determinado pacote:
```shell
apt-cache rdepends {{nome_do_pacote}}
```
{% endraw %}