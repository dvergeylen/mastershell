---
layout: default
title: "asdf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asdf">
  <a href="/pt_br/common/asdf.html">asdf</a> <a href="#asdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para a gestão de versões de linguagens e programas.
> Mais informações: <https://asdf-vm.com>.

#### Listar todos os plugins disponíveis:
```shell
asdf plugin-list-all
```
#### Instalar um plugin:
```shell
asdf plugin-add {{nome}}
```
#### Listar todas as versões disponíveis para um pacote:
```shell
asdf list-all {{nome}}
```
#### Instalar uma versão específica de um pacote:
```shell
asdf install {{nome}} {{versão}}
```
#### Definir a versão global de um pacote:
```shell
asdf global {{nome}} {{versão}}
```
#### Definir a versão local de um pacote:
```shell
asdf local {{nome}} {{versão}}
```
{% endraw %}