---
layout: default
title: "dokku"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dokku">
  <a href="/it/common/dokku.html">dokku</a> <a href="#dokku"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mini-Heroku basato su Docker (PaaS, Platform As A Service).
> Distribuisci facilmente molteplici app sul tuo server in diversi linguaggi utilizzando un singolo comando `git-push`.
> Maggiori informazioni: <https://github.com/dokku/dokku>.

#### Elenca app in esecuzione:
```shell
dokku apps
```
#### Crea un'app:
```shell
dokku apps:create {{nome_app}}
```
#### Rimuovi un'app:
```shell
dokku apps:destroy {{nome_app}}
```
#### Installa un plugin:
```shell
dokku plugin:install {{url_completo_repo}}
```
#### Collega un database ad un'app:
```shell
dokku {{db}}:link {{nome_db}} {{nome_app}}
```
{% endraw %}