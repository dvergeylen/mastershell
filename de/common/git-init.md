---
layout: default
title: "git init"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-init">
  <a href="/de/common/git-init.html">git init</a> <a href="#git-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstelle eine neues lokales Git-Repository.
> Weitere Informationen: <https://git-scm.com/docs/git-init>.

#### Erstelle eine neues lokales Repository:
```shell
git init
```
#### Erstelle ein neues Repository, welches SHA256 für Objekt-Hashes verwendet (benötigt Git 2.29+):
```shell
git init --object-format={{sha256}}
```
#### Erstelle eine neues minimales Repository, welches sich für die Verwendung als Remote-Repository über SSH eignet:
```shell
git init --bare
```
{% endraw %}