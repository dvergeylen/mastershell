---
layout: default
title: "add-apt-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="add-apt-repository">
  <a href="/it/linux/add-apt-repository.html">add-apt-repository</a> <a href="#add-apt-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisce le definizioni di repository apt.

#### Aggiunge un nuovo repository apt:
```shell
add-apt-repository {{identificativo_del_repository}}
```
#### Rimuove un repository apt:
```shell
add-apt-repository --remove {{identificativo_del_repository}}
```
#### Aggiorna la cache dei pacchetti dopo aver aggiunto un repository:
```shell
add-apt-repository --update {{identificativo_del_repository}}
```
#### Attiva i pacchetti sorgente:
```shell
add-apt-repository --enable-source {{identificativo_del_repository}}
```
{% endraw %}