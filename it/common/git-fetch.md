---
layout: default
title: "git fetch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-fetch">
  <a href="/it/common/git-fetch.html">git fetch</a> <a href="#git-fetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scarica oggetti e riferimenti da un repository remoto.
> Maggiori informazioni: <https://git-scm.com/docs/git-fetch>.

#### Scarica le ultime modifiche dal repository remoto di origine (upstream) di default, se definito:
```shell
git fetch
```
#### Scarica i nuovi rami da un dato repository remoto di origine:
```shell
git fetch {{nome_repository_remoto}}
```
#### Scarica le ultime modifiche da tutti i repository remoti di origine:
```shell
git fetch --all
```
#### Scarica anche i tag dal repository remoto di origine:
```shell
git fetch --tags
```
#### Elimina i riferimenti locali ai rami remoti che sono stati eliminati dal repositoy di origine:
```shell
git fetch --prune
```
{% endraw %}