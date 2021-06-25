---
layout: default
title: "git send-email"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-send-email">
  <a href="/fr/common/git-send-email.html">git send-email</a> <a href="#git-send-email"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Envoyer une collection de correctifs par email.
> Les correctifs peuvent être spécifiés sous forme de fichiers, de directions ou de liste de révisions.
> Plus d'informations : <https://git-scm.com/docs/git-send-email>.

#### Envoyer le dernier commit de la branche courante :
```shell
git send-email -1
```
#### envoyer un commit spécifique :
```shell
git send-email -1 {{commit}}
```
#### envoyer de multiples commits de la branche courante (ici : 10) :
```shell
git send-email {{-10}}
```
#### Envoyez un e-mail de présentation de la série de correctifs :
```shell
git send-email -{{number of commits}} --compose
```
#### Consultez et modifiez l'e-mail de chaque patch que vous êtes sur le point d'envoyer :
```shell
git send-email -{{number of commits}} --annotate
```
{% endraw %}