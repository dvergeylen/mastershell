---
layout: default
title: "atq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atq">
  <a href="/it/common/atq.html">atq</a> <a href="#atq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra job programmati dai comandi `at` o `batch`.
> Maggiori informazioni: <https://man.archlinux.org/man/at.1>.

#### Mostra i job programmati per l'utente corrente:
```shell
atq
```
#### Mostra i job della coda 'a' (le code hanno nomi di un singolo carattere):
```shell
atq -q {{a}}
```
#### Mostra i job di tutti gli utenti (da eseguire come super user):
```shell
sudo atq
```
{% endraw %}