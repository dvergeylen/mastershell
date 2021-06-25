---
layout: default
title: "apt-add-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-add-repository">
  <a href="/it/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisce le definizioni di repository apt.
> Maggiori informazioni: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Aggiunge un nuovo repository apt:
```shell
apt-add-repository {{identificativo_del_repository}}
```
#### Rimuove un repository apt:
```shell
apt-add-repository --remove {{identificativo_del_repository}}
```
#### Aggiorna la cache dei pacchetti dopo aver aggiunto un repository:
```shell
apt-add-repository --update {{identificativo_del_repository}}
```
#### Attiva i pacchetti sorgente:
```shell
apt-add-repository --enable-source {{identificativo_del_repository}}
```
{% endraw %}