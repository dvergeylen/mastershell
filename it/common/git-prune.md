---
layout: default
title: "git prune"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-prune">
  <a href="/it/common/git-prune.html">git prune</a> <a href="#git-prune"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina dal database degli oggetti quelli non più raggiungibili.
> Questo comando è usato più spesso internamente da Git gc piuttosto che in modo diretto.
> Maggiori informazioni: <https://git-scm.com/docs/git-prune>.

#### Elenca quali oggetti saranno eliminati da Git prune senza eliminarli definitivamente:
```shell
git prune --dry-run
```
#### Elimina gli oggetti non raggiungibili e stampane un elenco su stdout:
```shell
git prune --verbose
```
#### Elimina gli oggetti non raggiungibili, mostrando lo stato di avanzamento:
```shell
git prune --progress
```
{% endraw %}