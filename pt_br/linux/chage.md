---
layout: default
title: "chage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chage">
  <a href="/pt_br/linux/chage.html">chage</a> <a href="#chage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerencia informações de expiração de conta e senha do usuário.

#### Exibir as informações referentes a senha do usuário:
```shell
chage -l {{nome_do_usuario}}
```
#### Habilitar a expiração da senha do usuário em 10 dias:
```shell
sudo chage -M {{10}} {{nome_do_usuario}}
```
#### Desabilitar a expiração da senha do usuário:
```shell
sudo chage -M -1 {{nome_do_usuario}}
```
#### Definir a data de expiração da conta do usuário:
```shell
sudo chage -E {{YYYY-MM-DD}}
```
#### Obrigar o usuário a alterar sua senha no próximo login:
```shell
sudo chage -d 0
```
{% endraw %}