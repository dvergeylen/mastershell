---
layout: default
title: "authconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="authconfig">
  <a href="/pt_br/linux/authconfig.html">authconfig</a> <a href="#authconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interface de linha comandos para configurar o sistema de autenticação.

#### Exibir as configurações atuais (ou dry run):
```shell
authconfig --test
```
#### Configurar o servidor para utilizar diferentes algoritmos de hash para as senhas:
```shell
authconfig --update --passalgo={{algoritmo}}
```
#### Habilitar a autenticação via LDAP:
```shell
authconfig --update --enableldapauth
```
#### Desabilitar a autenticação via LDAP:
```shell
authconfig --update --disableldapauth
```
#### Habilitar o Network Information Service (NIS):
```shell
authconfig --update --enablenis
```
#### Habilitar Kerberos:
```shell
authconfig --update --enablekrb5
```
#### Habilitar a autenticação Winbind (Active Directory):
```shell
authconfig --update --enablewinbindauth
```
#### Habilitar a autorização local:
```shell
authconfig --update --enablelocauthorize
```
{% endraw %}