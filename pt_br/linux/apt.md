---
layout: default
title: "apt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt">
  <a href="/pt_br/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes das distribuições baseadas em Debian.
> Mais informações: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Atualizar a lista de pacotes disponíveis (recomenda-se executá-lo antes de outros comandos `apt`):
```shell
sudo apt update
```
#### Buscar pacotes correspondentes ao critério de busca:
```shell
apt search {{criterio_de_busca}}
```
#### Exibir as informações de pacote:
```shell
apt show {{nome_do_pacote}}
```
#### Instalar um pacote ou atualizá-lo para a versão mais recente:
```shell
sudo apt install {{nome_do_pacote}}
```
#### Remover um pacote (Para remover os arquivos de configuração deve-se usar a opção `purge` ao invés do `remove`):
```shell
sudo apt remove {{nome_do_pacote}}
```
#### Atualizar os pacotes instalados para as versões mais recentes:
```shell
sudo apt upgrade
```
{% endraw %}