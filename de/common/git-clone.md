---
layout: default
title: "git clone"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clone">
  <a href="/de/common/git-clone.html">git clone</a> <a href="#git-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Klone ein existierendes Repository.
> Weitere Informationen: <https://git-scm.com/docs/git-clone>.

#### Klone ein existierendes Repository:
```shell
git clone {{url_zu_repository}}
```
#### Klone ein existierendes Repository in ein bestimmtes Verzeichnis:
```shell
git clone {{url_zu_repository}} {{pfad/zu/verzeichnis}}
```
#### Klone ein existierendes Repository und seine Submodule:
```shell
git clone --recursive {{url_zu_repository}}
```
#### Klone ein lokales Repository:
```shell
git clone -l {{pfad/zu/lokalem_repository}}
```
#### Klone ohne Meldungen:
```shell
git clone -q {{url_zu_repository}}
```
#### Klone ein existierendes Repository und rufe nur die neuesten 10 Commits im Standard-Branch ab (spart Zeit):
```shell
git clone --depth {{10}} {{url_zu_repository}}
```
#### Klone ein existierendes Repository, aber lade nur einen bestimmten Branch herunter:
```shell
git clone --branch {{name}} --single-branch {{url_zu_repository}}
```
{% endraw %}