---
layout: default
title: "git remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-remote">
  <a href="/it/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci i collegamenti remoti ("remote") di un repository locale.
> Maggiori informazioni: <https://git-scm.com/docs/git-remote>.

#### Mostra l'elenco dei collegamenti remoti, con il loro nome e URL:
```shell
git remote -v
```
#### Mostra informazioni su un remote:
```shell
git remote show {{nome_remote}}
```
#### Aggiungi un remote:
```shell
git remote add {{nome_remote}} {{url_remote}}
```
#### Modifica l'URL di un remote (usa `--add` per preservare gli URL esistenti):
```shell
git remote set-url {{nome_remoto}} {{nuovo_url}}
```
#### Elimina un remote:
```shell
git remote remove {{nome_remote}}
```
#### Rinomina un remote:
```shell
git remote rename {{vecchio_nome}} {{nuovo_nome}}
```
{% endraw %}