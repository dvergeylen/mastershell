---
layout: default
title: "autorandr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autorandr">
  <a href="/pt_br/linux/autorandr.html">autorandr</a> <a href="#autorandr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Altera o layout da tela automaticamente.

#### Salvar o layout da tela em uso:
```shell
autorandr -s {{nome_do_perfil}}
```
#### Exibir os perfis salvos:
```shell
autorandr
```
#### Alterar o perfil:
```shell
autorandr -l {{nome_do_perfil}}
```
#### Definir o perfil padrão:
```shell
autorandr -d {{nome_do_perfil}}
```
{% endraw %}