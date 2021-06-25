---
layout: default
title: "adduser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adduser">
  <a href="/pt_br/linux/adduser.html">adduser</a> <a href="#adduser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para criação de novos usuários.
> Mais informações: <https://manpages.debian.org/latest/adduser/adduser.html>.

#### Criar um novo usuário, o seu diretório na pasta home e solicitar o preenchimento da sua senha:
```shell
adduser {{nome_do_usuario}}
```
#### Criar um novo usuário sem o seu diretório na pasta home:
```shell
adduser --no-create-home {{nome_do_usuario}}
```
#### Criar um novo usuário especificando a localização do seu diretório:
```shell
adduser --home {{caminho_da_pasta_do_usuario}} {{nome_do_usuario}}
```
#### Criar um novo usuário e configurar o seu shell de login:
```shell
adduser --shell {{caminho_para_o_shell}} {{nome_do_usuario}}
```
#### Criar um novo usuário e atribuí-lo a um grupo:
```shell
adduser --ingroup {{grupo}} {{nome_do_usuario}}
```
{% endraw %}