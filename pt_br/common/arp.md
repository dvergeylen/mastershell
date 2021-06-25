---
layout: default
title: "arp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arp">
  <a href="/pt_br/common/arp.html">arp</a> <a href="#arp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostrar e manipular a cache ARP do sistema.
> Mais informações: <https://manned.org/arp>.

#### Mostrar a tabela arp atual:
```shell
arp -a
```
#### Limpar toda a cache:
```shell
sudo arp -a -d
```
#### Eliminar uma entrada específica:
```shell
arp -d {{endereço}}
```
#### Criar uma entrada:
```shell
arp -s {{endereço}} {{endereço_mac}}
```
{% endraw %}