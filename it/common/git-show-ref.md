---
layout: default
title: "git show-ref"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show-ref">
  <a href="/it/common/git-show-ref.html">git show-ref</a> <a href="#git-show-ref"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elenca i riferimenti.
> Maggiori informazioni: <https://git-scm.com/docs/git-show-ref>.

#### Mostra tutti i riferimenti nel repository:
```shell
git show-ref
```
#### Mostra solo i riferimenti agli HEAD:
```shell
git show-ref --heads
```
#### Mostra solo i riferimenti ai tag:
```shell
git show-ref --tags
```
#### Verifica che un certo riferimento esista:
```shell
git show-ref --verify {{percorso/al/riferimento}}
```
{% endraw %}