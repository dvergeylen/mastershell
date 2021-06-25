---
layout: default
title: "gopass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gopass">
  <a href="/en/common/gopass.html">gopass</a> <a href="#gopass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Standard Unix Password Manager for Teams. Written in Go.
> More information: <https://www.gopass.pw>.

#### Initialise the configuration settings:
```shell
gopass init
```
#### Create a new entry:
```shell
gopass new
```
#### Show all stores:
```shell
gopass mounts
```
#### Mount a shared Git store:
```shell
gopass mounts add {{store_name}} {{git_repo_url}}
```
#### Search interactively using a keyword:
```shell
gopass show {{keyword}}
```
#### Search using a keyword:
```shell
gopass find {{keyword}}
```
#### Sync all mounted stores:
```shell
gopass sync
```
#### Show a particular password entry:
```shell
gopass {{store_name|path/to/directory|email@email.com}}
```
{% endraw %}