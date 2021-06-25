---
layout: default
title: "git archive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-archive">
  <a href="/it/common/git-archive.html">git archive</a> <a href="#git-archive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea un archivio dei file nell'albero di lavoro.
> Maggiori informazioni: <https://git-scm.com/docs/git-archive>.

#### Crea un archivio tar del contenuto in HEAD e stampa il risultato su standard output:
```shell
git archive --verbose HEAD
```
#### Crea un archivio zip del contenuto in HEAD e stampa il risultato su standard output:
```shell
git archive --verbose --format=zip HEAD
```
#### Come sopra, ma scrivi l'archivio zip su file:
```shell
git archive --verbose --output={{percorso/al/file.zip}} HEAD
```
#### Crea un archivio tar dell'ultimo commit sul ramo specificato:
```shell
git archive --output={{percorso/al/file.tar}} {{nome_ramo}}
```
#### Crea un archivio tar del contenuto di una specifica cartella:
```shell
git archive --output={{percorso/al/file.tar}} HEAD:{{percorso/alla/directory}}
```
#### Anteponi un percorso ad ogni file cosí da archiviarlo in una cartella specifica:
```shell
git archive --output={{percorso/al/file.tar}} --prefix={{percorso/da/anteporre}}/ HEAD
```
{% endraw %}