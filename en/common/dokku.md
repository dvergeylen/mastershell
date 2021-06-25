---
layout: default
title: "dokku"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dokku">
  <a href="/en/common/dokku.html">dokku</a> <a href="#dokku"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker powered mini-Heroku (PaaS).
> Easily deploy multiple apps to your server in different languages using a single `git-push` command.
> More information: <https://github.com/dokku/dokku>.

#### List running apps:
```shell
dokku apps
```
#### Create an app:
```shell
dokku apps:create {{app_name}}
```
#### Remove an app:
```shell
dokku apps:destroy {{app_name}}
```
#### Install plugin:
```shell
dokku plugin:install {{full_repo_url}}
```
#### Link database to an app:
```shell
dokku {{db}}:link {{db_name}} {{app_name}}
```
{% endraw %}