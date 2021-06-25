---
layout: default
title: "chkconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chkconfig">
  <a href="/pt_br/linux/chkconfig.html">chkconfig</a> <a href="#chkconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerencia o runlevel dos serviços no CentOS 6.

#### Exibir os serviços com os respectivos runlevels:
```shell
chkconfig --list
```
#### Exibir o runlevel de um serviço:
```shell
chkconfig --list {{ntpd}}
```
#### Habilitar o início de um serviço durante o processo de boot:
```shell
chkconfig {{sshd}} on
```
#### Habilitar o início do serviço durante o processo de boot para os runlevels 2, 3, 4 e 5:
```shell
chkconfig --level {{2345}} {{sshd}} on
```
#### Desabilitar a inicialização de um determinado serviço durante o processo de boot:
```shell
chkconfig {{ntpd}} off
```
#### Desabilitar a inicialização de um determinado serviço durante o processo de boot para o runlevel 3:
```shell
chkconfig --level {{3}} {{ntpd}} off
```
{% endraw %}