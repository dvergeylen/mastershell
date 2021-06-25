---
layout: default
title: "git restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-restore">
  <a href="/it/common/git-restore.html">git restore</a> <a href="#git-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ripristina i file dell'albero di lavoro. Richiede versioni di Git successive alla 2.23.
> Vedi anche `git checkout`.
> Maggiori informazioni: <https://git-scm.com/docs/git-restore>.

#### Ripristina un file cancellato dal contenuto del commit corrente (HEAD):
```shell
git restore {{percorso/al/file}}
```
#### Ripristina un file alla versione di un commit differente:
```shell
git restore --source {{commit}} {{percorso/al/file}}
```
#### Annulla le modifiche ai file nell'area di stage, ripristinandoli all'HEAD:
```shell
git restore .
```
{% endraw %}