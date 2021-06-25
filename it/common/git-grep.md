---
layout: default
title: "git-grep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-grep">
  <a href="/it/common/git-grep.html">git-grep</a> <a href="#git-grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cerca stringhe nello storico dei file tracciati nel repository.
> Supporta molti degli stessi parametri accettati dal comando `grep` tradizionale.
> Maggiori informazioni: <https://git-scm.com/docs/git-grep>.

#### Cerca una stringa nei file tracciati:
```shell
git grep {{stringa_ricercata}}
```
#### Cerca una stringa nei file tracciati che soddisfano un dato pattern:
```shell
git grep {{stringa_ricercata}} -- {{file_glob_pattern}}
```
#### Cerca una stringa nei file tracciati, sottomoduli inclusi:
```shell
git grep --recurse-submodules {{stringa_ricercata}}
```
#### Cerca una stringa in uno dato momento della cronologia del repository:
```shell
git grep {{stringa_ricercata}} {{HEAD~2}}
```
#### Cerca una stringa in tutti i rami:
```shell
git grep {{stringa_ricercata}} $(git rev-list --all)
```
{% endraw %}