---
layout: default
title: "dpkg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dpkg">
  <a href="/it/linux/dpkg.html">dpkg</a> <a href="#dpkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di pacchetti Debian.
> Maggiori informazioni: <https://manpages.debian.org/buster/dpkg/dpkg.1.en.html>.

#### Installa un pacchetto:
```shell
dpkg -i {{percorso/al/file.deb}}
```
#### Rimuove un pacchetto:
```shell
dpkg -r {{nome_del_pacchetto}}
```
#### Elenca i pacchetti installati:
```shell
dpkg -l {{espressione_per_la_ricerca}}
```
#### Elenca i contenuti di un pacchetto:
```shell
dpkg -L {{nome_del_pacchetto}}
```
#### Elenca i contenuti di un file pacchetto locale:
```shell
dpkg -c {{percorso/al/file.deb}}
```
#### Trova a quale pacchetto appartiene un file:
```shell
dpkg -S {{filename}}
```
{% endraw %}