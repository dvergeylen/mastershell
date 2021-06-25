---
layout: default
title: "lambo new"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lambo-new">
  <a href="/en/common/lambo-new.html">lambo new</a> <a href="#lambo-new"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A super-powered `laravel new` for Laravel and Valet.
> More information: <https://github.com/tighten/lambo>.

#### Create a new Laravel application:
```shell
lambo new {{app_name}}
```
#### Install the application in a specific path:
```shell
lambo new --path={{path/to/directory}} {{app_name}}
```
#### Include authentication scaffolding:
```shell
lambo new --auth {{app_name}}
```
#### Include a specific frontend:
```shell
lambo new --{{vue|bootstrap|react}} {{app_name}}
```
#### Install npm dependencies after the project has been created:
```shell
lambo new --node {{app_name}}
```
#### Create a Valet site after the project has been created:
```shell
lambo new --link {{app_name}}
```
#### Create a new MySQL database with the same name as the project:
```shell
lambo new --create-db --dbuser={{user}} --dbpassword={{password}} {{app_name}}
```
#### Open a specific editor after the project has been created:
```shell
lambo new --editor="{{editor}}" {{app_name}}
```
{% endraw %}