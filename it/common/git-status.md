---
layout: default
title: "git status"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-status">
  <a href="/it/common/git-status.html">git status</a> <a href="#git-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra le modifiche ai file in un repository Git.
> Elenca i file modificati, aggiunti e cancellati rispetto al commit corrente.
> Maggiori informazioni: <https://git-scm.com/docs/git-status>.

#### Mostra i file modificati che non sono stati ancora committati:
```shell
git status
```
#### Mostra l'output in formato ridotto:
```shell
git status -s
```
#### Nascondi i file non tracciati dall'output:
```shell
git status --untracked-files=no
```
#### Mostra informazioni sul ramo ed in formato ridotto:
```shell
git status -sb
```
{% endraw %}