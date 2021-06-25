---
layout: default
title: "git remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-remote">
  <a href="/de/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte eine gewisse Anzahl an Repositories (remotes).
> Weitere Informationen: <https://git-scm.com/docs/git-remote>.

#### Liste alle existierenden Remotes, ihre Namen und ihre URLs auf:
```shell
git remote -v
```
#### Zeige Informationen über ein Remote an:
```shell
git remote show {{remote_name}}
```
#### Füge ein neues Remote hinzu:
```shell
git remote add {{remote_name}} {{remote_url}}
```
#### Ändere die URL eines Remotes (benutze `--add` um die existierende URL zu behalten):
```shell
git remote set-url {{remote_name}} {{remote_url}}
```
#### Entferne ein Remote:
```shell
git remote remove {{remote_name}}
```
#### Benenne ein Remote um:
```shell
git remote rename {{alter_name}} {{neuer_name}}
```
{% endraw %}