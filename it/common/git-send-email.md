---
layout: default
title: "git send-email"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-send-email">
  <a href="/it/common/git-send-email.html">git send-email</a> <a href="#git-send-email"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Invia una raccolta di patch via email.
> Le patch possono essere specificate come file, cartelle, o liste di revisione.
> Maggiori informazioni: <https://git-scm.com/docs/git-send-email>.

#### Invia l'ultimo commit nel ramo corrente:
```shell
git send-email -1
```
#### Invia un commit specifico:
```shell
git send-email -1 {{commit}}
```
#### Invia 10 commit nel ramo corrente:
```shell
git send-email {{-10}}
```
#### Invia un'email con un messaggio introduttivo alla serie di patch:
```shell
git send-email -{{numero_di_commit}} --compose
```
#### Revisiona e modifica il messaggio email per ogni patch da inviare:
```shell
git send-email -{{numero_di_commit}} --annotate
```
{% endraw %}