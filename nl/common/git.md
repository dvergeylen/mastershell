---
layout: default
title: "git"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git">
  <a href="/nl/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gedistribueerd versiebeheersysteem.
> Meer informatie: <https://git-scm.com/>.

#### Controleer de Git versie:
```shell
git --version
```
#### Toon algemene hulp:
```shell
git --help
```
#### Toon hulp bij een Git-subcommando (zoals `commit`, `log`, enz.):
```shell
git help {{subcommando}}
```
#### Voer een Git-subcommando uit:
```shell
git {{subcommando}}
```
#### Voer een Git-subcommando uit op een aangepast repository-rootpad:
```shell
git -C {{pad/naar/repo}} {{subcommando}}
```
#### Voer een Git-subcommando met een gegeven configuratieset:
```shell
git -c '{{config.sleutel}}={{waarde}}' {{subcommando}}
```
{% endraw %}