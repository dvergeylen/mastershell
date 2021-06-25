---
layout: default
title: "git cat-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cat-file">
  <a href="/it/common/git-cat-file.html">git cat-file</a> <a href="#git-cat-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visualizza il contenuto di un oggetto Git nel repository o mostrane dimensione e tipo.
> Maggiori informazioni: <https://git-scm.com/docs/git-cat-file>.

#### Mostra la dimen[s]ione del commit HEAD in byte:
```shell
git cat-file -s HEAD
```
#### Mostra il [t]ipo (blob, albero, commit, tag) di un oggetto Git:
```shell
git cat-file -t {{8c442dc3}}
```
#### Stam[p]a il contenuto di un oggetto Git, formattato in base al tipo:
```shell
git cat-file -p {{HEAD~2}}
```
{% endraw %}