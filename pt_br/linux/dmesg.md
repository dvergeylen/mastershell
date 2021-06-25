---
layout: default
title: "dmesg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmesg">
  <a href="/pt_br/linux/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Escreve as mensagens do kernel na terminal.

#### Exibir as mensagens do kernel:
```shell
dmesg
```
#### Exibir as mensagens de erro do kernel:
```shell
dmesg --level err
```
#### Exibir as mensagens do kernel e manter o terminal esperando por novas menagens, semelhante ao `tail -f` (disponível nas versões 3.5.0 e superiores do kernel):
```shell
dmesg -w
```
#### Exibir a quantidade de memória física disponível no sistema:
```shell
dmesg | grep -i memory
```
#### Exibir as mensagens do kernel divididas em páginas:
```shell
dmesg | less
```
#### Exibir as menagens do kernel com data/hora (disponível nas versões 3.5.0 e superiores do kernel):
```shell
dmesg -T
```
#### Exibir as mensagens do kernel em um formato de fácil leitura (disponível nas versões 3.5.0 e superiores do kernel):
```shell
dmesg -H
```
#### Exibir as mensagens do kernel utilizando cores (disponível nas versões 3.5.0 e superiores do kernel):
```shell
dmesg -L
```
{% endraw %}