---
layout: default
title: "apk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apk">
  <a href="/pt_br/linux/apk.html">apk</a> <a href="#apk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de pacotes da distribuição Alpine.

#### Atualizar os índices dos pacotes disponíveis:
```shell
apk update
```
#### Instalar um pacote:
```shell
apk add {{pacote}}
```
#### Remover um pacote:
```shell
apk del {{pacote}}
```
#### Reparar ou atualizar um pacote sem modificar as principais dependências:
```shell
apk fix {{pacote}}
```
#### Procurar um pacote especificando alguma palavra-chave:
```shell
apk search {{palavra_chave}}
```
#### Exibir informações sobre um pacote:
```shell
apk info {{pacote}}
```
{% endraw %}