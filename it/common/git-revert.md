---
layout: default
title: "git revert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-revert">
  <a href="/it/common/git-revert.html">git revert</a> <a href="#git-revert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea nuovi commit che invertano i risultati dei commit precedenti.
> Maggiori informazioni: <https://git-scm.com/docs/git-revert>.

#### Inverti il commit più recente:
```shell
git revert {{@}}
```
#### Inverti il quintùltimo commit:
```shell
git revert HEAD~{{4}}
```
#### Inverti più commit:
```shell
git revert {{nome_ramo~5..nome_ramo~2}}
```
#### Inverti senza creare nuovi commit, ma modificando l'albero di lavoro:
```shell
git revert -n {{0c01a9..9a1743}}
```
{% endraw %}