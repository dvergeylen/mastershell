---
layout: default
title: "arp-scan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arp-scan">
  <a href="/pt_br/linux/arp-scan.html">arp-scan</a> <a href="#arp-scan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Envia pacotes ARP para máquinas (identificadas por endereço IP ou por nome de domínio) em uma rede local, identificando as máquinas ativas de acordo com as respostas.

#### Verificar as máquinas da rede local:
```shell
arp-scan --localnet
```
#### Verificar as máquinas de uma rede IP especificando a máscara de bit:
```shell
arp-scan {{192.168.1.1}}/{{24}}
```
#### Verificar as máquinas de uma rede IP que estejam em uma faixa de valores:
```shell
arp-scan {{127.0.0.0}}-{{127.0.0.31}}
```
#### Verificar as máquinas de uma rede IP especificando a máscara de rede:
```shell
arp-scan {{10.0.0.0}}:{{255.255.255.0}}
```
{% endraw %}