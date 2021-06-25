---
layout: default
title: "git push"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-push">
  <a href="/it/common/git-push.html">git push</a> <a href="#git-push"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Invia i commit a un repository remoto.
> Maggiori informazioni: <https://git-scm.com/docs/git-push>.

#### Invia le modifiche fatte nel ramo corrente locale al corrispondente ramo remoto:
```shell
git push
```
#### Invia le modifiche fatte in uno specifico ramo locale al corrispondente ramo remoto:
```shell
git push {{nome_repository_remoto}} {{nome_ramo}}
```
#### Pubblica il ramo corrente in un repository remoto, specificando il nome del ramo remoto:
```shell
git push {{nome_repository_remoto}} -u {{nome_ramo_remoto}}
```
#### Invia le modifiche fatte in ogni ramo locale ai corrispondenti rami remoti:
```shell
git push --all {{nome_repository_remoto}}
```
#### Cancella un ramo di un repository remoto:
```shell
git push {{nome_repository_remoto}} --delete {{nome_ramo_remoto}}
```
#### Cancella i rami remoti che non hanno un ramo locale corrispondente:
```shell
git push --prune {{nome_repository_remoto}}
```
#### Pubblica i tag che non sono già presenti nel repository remoto:
```shell
git push --tags
```
{% endraw %}