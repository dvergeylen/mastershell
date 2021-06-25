---
layout: default
title: "git gc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-gc">
  <a href="/it/common/git-gc.html">git gc</a> <a href="#git-gc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ottimizza il repository locale ripulendolo dai file non necessari.
> Maggiori informazioni: <https://git-scm.com/docs/git-gc>.

#### Ottimizza il repository:
```shell
git gc
```
#### Ottimizza il repository in modo più aggressivo, impiegando più tempo:
```shell
git gc --aggressive
```
#### Non eliminare gli oggetti non tracciati (sono eliminati di default):
```shell
git gc --no-prune
```
#### Non mostrare alcun output:
```shell
git gc --quiet
```
#### Mostra utilizzo completo:
```shell
git gc --help
```
{% endraw %}