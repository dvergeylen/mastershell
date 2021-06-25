---
layout: default
title: "git format-patch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-format-patch">
  <a href="/it/common/git-format-patch.html">git format-patch</a> <a href="#git-format-patch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prepara file .patch. Utile per l'invio di commit via email.
> Vedi anche `git am`, che permette di applicare file .patch.
> Maggiori informazioni: <https://git-scm.com/docs/git-format-patch>.

#### Crea un file `.patch` (il nome è assegnato automaticamente) con i commit non ancora inviati al repository remoto:
```shell
git format-patch {{origin}}
```
#### Scrivi su stdout un file `.patch` per l'intervallo di commit definito dai due commit dati:
```shell
git format-patch --stdout {{commit_1}}..{{commit_2}}
```
#### Scrivi un file `.patch` per gli ultimi 3 commit:
```shell
git format-patch -{{3}}
```
{% endraw %}