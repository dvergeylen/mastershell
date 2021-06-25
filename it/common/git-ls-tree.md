---
layout: default
title: "git ls-tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ls-tree">
  <a href="/it/common/git-ls-tree.html">git ls-tree</a> <a href="#git-ls-tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elenca il contenuto di un oggetto albero.
> Maggiori informazioni: <https://git-scm.com/docs/git-ls-tree>.

#### Mostra il contenuto dell'albero su un ramo:
```shell
git ls-tree {{nome_ramo}}
```
#### Mostra il contenuto dell'albero su un commit, procedendo ricorsivamente nei sotto-alberi:
```shell
git ls-tree -r {{hash_commit}}
```
#### Mostra solo il nome dei file dell'albero su un commit:
```shell
git ls-tree --name-only {{hash_commit}}
```
{% endraw %}