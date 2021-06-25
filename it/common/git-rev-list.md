---
layout: default
title: "git rev-list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rev-list">
  <a href="/it/common/git-rev-list.html">git rev-list</a> <a href="#git-rev-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elenca le revisioni (commit) in ordine cronologico inverso.
> Maggiori informazioni: <https://git-scm.com/docs/git-rev-list>.

#### Mostra tutti i commit del ramo corrente:
```shell
git rev-list {{HEAD}}
```
#### Mostra i commit più recenti di una certa data, su uno specifico ramo:
```shell
git rev-list --since={{'2019-12-01 00:00:00'}} {{nome_ramo}}
```
#### Mostra tutti i commit di unione (merge commit) associati a uno specifico commit:
```shell
git rev-list --merges {{commit}}
```
{% endraw %}