---
layout: default
title: "dpkg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dpkg">
  <a href="/pt_br/linux/dpkg.html">dpkg</a> <a href="#dpkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes Debian.

#### Instalar um pacote:
```shell
dpkg -i {{arquivo.deb}}
```
#### Remover um pacote:
```shell
dpkg -r {{nome_do_pacote}}
```
#### Exibir os pacotes correspondentes ao critério de busca:
```shell
dpkg -l {{criterio_de_busca}}
```
#### Exibe o conteúdo do pacote:
```shell
dpkg -L {{nome_do_pacote}}
```
#### Exibir o conteúdo do arquivo de um pacote:
```shell
dpkg -c {{arquivo.deb}}
```
#### Apresentar o pacote proprietário de um determinado arquivo:
```shell
dpkg -S {{nome_do_arquivo}}
```
{% endraw %}