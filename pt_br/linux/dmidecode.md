---
layout: default
title: "dmidecode"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmidecode">
  <a href="/pt_br/linux/dmidecode.html">dmidecode</a> <a href="#dmidecode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe em formato de fácil leitura o sumário DMI (também conhecido como SMBIOS) .
> Requer privilégio de super usuário.

#### Exibir o sumário do DMI:
```shell
sudo dmidecode
```
#### Exibir a versão da BIOS:
```shell
sudo dmidecode -s bios-version
```
#### Exibir o número de série do sistema:
```shell
sudo dmidecode -s system-serial-number
```
#### Exibir as informações da BIOS:
```shell
sudo dmidecode -t bios
```
#### Exibir as informações da CPU:
```shell
sudo dmidecode -t processor
```
#### Exibir as informações da memória:
```shell
sudo dmidecode -t memory
```
{% endraw %}