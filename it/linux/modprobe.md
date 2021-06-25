---
layout: default
title: "modprobe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="modprobe">
  <a href="/it/linux/modprobe.html">modprobe</a> <a href="#modprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aggiunge o rimuove moduli del kernel Linux.

#### Fa finta di carica un modulo nel kernel, ma non lo fa veramente:
```shell
sudo modprobe --dry-run {{nome_del_modulo}}
```
#### Carica un modulo nel kernel:
```shell
sudo modprobe {{nome_del_modulo}}
```
#### Rimuove un modulo dal kernel:
```shell
sudo modprobe --remove {{nome_del_modulo}}
```
#### Rimuove dal kernel un modulo e quelli che dipendono da quest'ultimo:
```shell
sudo modprobe --remove-dependencies {{nome_del_modulo}}
```
#### Mostra le dipendenza di un modulo del kernel:
```shell
sudo modprobe --show-depends {{nome_del_modulo}}
```
{% endraw %}