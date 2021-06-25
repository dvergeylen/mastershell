---
layout: default
title: "lsusb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsusb">
  <a href="/it/linux/lsusb.html">lsusb</a> <a href="#lsusb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visualizza le informazioni su i bus USB e i dispositivi a loro connessi.

#### Elenca tutti i dispositivi USB disponibili:
```shell
lsusb
```
#### Visualizza la gerarchia USB come un albero:
```shell
lsusb -t
```
#### Elenca informazioni prolisse riguardo ai dispositivi USB:
```shell
lsusb --verbose
```
#### Elenca informazioni dettagliate riguardo ad un dispositivo USB:
```shell
lsusb -D {{dispositivo}}
```
#### Elenca solamente i dispositivi con un certo id fornitore e id prodotto:
```shell
lsusb -d {{fornitore}}:{{prodotto}}
```
{% endraw %}