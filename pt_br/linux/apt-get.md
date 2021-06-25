---
layout: default
title: "apt-get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-get">
  <a href="/pt_br/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes das distribuições baseadas em Debian.
> Procure por pacotes utilizando o `apt-cache`.
> Mais informações: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Atualizar a lista de pacotes disponíveis (recomenda-se executá-lo antes de outros comandos `apt-get`):
```shell
apt-get update
```
#### Instalar um pacote ou atualizá-lo para a versão mais recente:
```shell
apt-get install {{nome_do_pacote}}
```
#### Remover um pacote:
```shell
apt-get remove {{nome_do_pacote}}
```
#### Remover um pacote e os seus arquivos de configuração:
```shell
apt-get purge {{nome_do_pacote}}
```
#### Atualizar todos os pacotes instalados para as versões mais recentes:
```shell
apt-get upgrade
```
#### Limpar o repositório local — removendo os arquivos de pacotes (`.deb`) de downloads interrompidos que não podem mais ser baixados:
```shell
apt-get autoclean
```
#### Remover todos os pacotes obsoletos:
```shell
apt-get autoremove
```
#### Atualizar os pacotes instalados (semelhante ao `upgrade`), porém removendo os obsoletos e instalando pacotes solicitados por novas dependências:
```shell
apt-get dist-upgrade
```
{% endraw %}