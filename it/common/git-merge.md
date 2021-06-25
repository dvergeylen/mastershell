---
layout: default
title: "git merge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-merge">
  <a href="/it/common/git-merge.html">git merge</a> <a href="#git-merge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui un'unione (merge) tra due rami Git.
> Maggiori informazioni: <https://github.com/mhagger/git-merge>.

#### Avvia un'unione con il tuo ramo corrente:
```shell
git merge {{ramo_da_unire}}
```
#### Avvia un'unione e cambia il messaggio predefinito:
```shell
git merge --edit {{ramo_da_unire}}
```
#### Avvia un'unione e committa l'operazione:
```shell
git merge --no-ff {{ramo_da_unire}}
```
#### Interrompi un'unione in caso di conflitti:
```shell
git merge --abort
```
{% endraw %}