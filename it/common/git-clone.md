---
layout: default
title: "git clone"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clone">
  <a href="/it/common/git-clone.html">git clone</a> <a href="#git-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clona un repository esistente.
> Maggiori informazioni: <https://git-scm.com/docs/git-clone>.

#### Clona un repository remoto esistente:
```shell
git clone {{url_repository_remoto}}
```
#### Clona un repository remoto insieme ai suoi sottomoduli:
```shell
git clone --recursive {{url_repository_remoto}}
```
#### Clona un repository locale:
```shell
git clone -l {{percorso/a/repository/locale}}
```
#### Clona in modalità silenziosa:
```shell
git clone -q {{url_repository_remoto}}
```
#### Clona un repository remoto scaricando solo i 10 commit più recenti del ramo principale (utile per risparmiare tempo):
```shell
git clone --depth {{10}} {{url_repository_remoto}}
```
{% endraw %}