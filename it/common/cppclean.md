---
layout: default
title: "cppclean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cppclean">
  <a href="/it/common/cppclean.html">cppclean</a> <a href="#cppclean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trova codice inutilizzato in progetti C++.
> Maggiori informazioni: <https://github.com/myint/cppclean>.

#### Esegui nella directory di un progetto:
```shell
cppclean {{percorso/a/directory_progetto}}
```
#### Esegui su di un progetto dove gli header sono nella directory "inc1" ed "inc2":
```shell
cppclean {{percorso/a/directory_progetto}} --include-path={{inc1}} --include-path={{inc2}}
```
#### Esegui su di uno specifico file `main.cpp`:
```shell
cppclean {{main.cpp}}
```
#### Esegui della directory corrente, escludendo la directory "build":
```shell
cppclean {{.}} --exclude={{build}}
```
{% endraw %}