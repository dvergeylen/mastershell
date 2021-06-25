---
layout: default
title: "git mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-mv">
  <a href="/it/common/git-mv.html">git mv</a> <a href="#git-mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sposta o rinomina file e aggiorna l'indice Git.
> Maggiori informazioni: <https://git-scm.com/docs/git-mv>.

#### Sposta i file nella repository e aggiungi l'operazione al commit successivo:
```shell
git mv {{percorso/al/file}} {{nuovo/percorso/al/file}}
```
#### Rinomina i file e aggiungi l'operazione al commit successivo:
```shell
git mv {{file}} {{file_rinominato}}
```
#### Sposta sovrascrivendo eventuali file esistenti nel percorso di destinazione:
```shell
git mv --force {{percorso/al/file}} {{nuovo/percorso/al/file}}
```
{% endraw %}