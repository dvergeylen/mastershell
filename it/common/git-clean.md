---
layout: default
title: "git clean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clean">
  <a href="/it/common/git-clean.html">git clean</a> <a href="#git-clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina i file non tracciati dall'albero di lavoro.
> Maggiori informazioni: <https://git-scm.com/docs/git-clean>.

#### Elimina i file che non sono tracciati da Git:
```shell
git clean
```
#### Elimina in modo interattivo i file non tracciati da Git:
```shell
git clean -i
```
#### Mostra quali file non tracciati sarebbero eliminati, senza però eliminarli davvero:
```shell
git clean --dry-run
```
#### Forza l'eliminazione dei file non tracciati da Git:
```shell
git clean -f
```
#### Forza l'eliminazione delle cartelle non tracciate da Git:
```shell
git clean -fd
```
#### Elimina i file non tracciati, compresi quelli da ignorare elencati in `.gitignore` e `.git/info/exclude`:
```shell
git clean -x
```
{% endraw %}