---
layout: default
title: "git replace"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-replace">
  <a href="/it/common/git-replace.html">git replace</a> <a href="#git-replace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea, elenca, ed elimina riferimenti ad oggetti sostituiti.
> Maggiori informazioni: <https://git-scm.com/docs/git-replace>.

#### Sostituisci un commit con un altro, senza modificare gli altri commit:
```shell
git replace {{oggetto}} {{oggetto_sostitutivo}}
```
#### Cancella riferimenti esistenti ad un oggetto sostituito:
```shell
git replace --delete {{oggetto}}
```
#### Modifica il contenuto di un oggetto in modo interattivo:
```shell
git replace --edit {{oggetto}}
```
{% endraw %}