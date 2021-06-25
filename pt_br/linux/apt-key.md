---
layout: default
title: "apt-key"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-key">
  <a href="/pt_br/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de chaves utilizado pelo gerenciador de pacotes APT nas distribuições baseadas em Debian.
> Mais informações: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### Exibir as chaves confiáveis:
```shell
apt-key list
```
#### Adicionar uma chave na lista de chaves confiáveis:
```shell
apt-key add {{arquivo_da_chave_publica.asc}}
```
#### Remover uma chave da lista de chaves confiáveis:
```shell
apt-key del {{key_id}}
```
#### Adicionar uma chave remota na lista de chaves confiáveis:
```shell
wget -qO - {{https://host.tld/arquivo.key}} | apt-key add -
```
#### Adicionar uma chave, de um servidor de chaves, na lista de chaves confiáveis:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{KEYID}}
```
{% endraw %}