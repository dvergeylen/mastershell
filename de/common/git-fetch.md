---
layout: default
title: "git fetch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-fetch">
  <a href="/de/common/git-fetch.html">git fetch</a> <a href="#git-fetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lade Objekte und Referenzen (refs) von einem entfernten Repository.
> Weitere Informationen: <https://git-scm.com/docs/git-fetch>.

#### Hole die neuesten Änderungen von dem standardmäßigen Repository im Upstream (wenn gesetzt):
```shell
git fetch
```
#### Hole neue Branches von einem bestimmten Repository im Upstream:
```shell
git fetch {{name_des_upstream_repository}}
```
#### Hole die neuesten Änderungen von allen Repositories im Upstream:
```shell
git fetch --all
```
#### Lade auch die Tags des Repository im Upstream:
```shell
git fetch --tags
```
#### Lösche lokale Referenzen auf entfernte Branches, die im Upstream-Repository nicht mehr existieren:
```shell
git fetch --prune
```
{% endraw %}