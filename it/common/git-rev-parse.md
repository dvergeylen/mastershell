---
layout: default
title: "git rev-parse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rev-parse">
  <a href="/it/common/git-rev-parse.html">git rev-parse</a> <a href="#git-rev-parse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra i metadati relativi a specifiche revisioni.
> Maggiori informazioni: <https://git-scm.com/docs/git-rev-parse>.

#### Mostra l'hash del commit di un ramo:
```shell
git rev-parse {{nome_ramo}}
```
#### Mostra il nome del ramo corrente:
```shell
git rev-parse --abbrev-ref {{HEAD}}
```
#### Mostra il percorso assoluto della cartella di root:
```shell
git rev-parse --show-toplevel
```
{% endraw %}