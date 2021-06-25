---
layout: default
title: "git status"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-status">
  <a href="/de/common/git-status.html">git status</a> <a href="#git-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige die Änderungen an Dateien in einem Git-Repository an.
> Weitere Informationen: <https://git-scm.com/docs/git-status>.

#### Zeige veränderte Dateien an, die noch nicht für den Commit hinzugefügt wurden:
```shell
git status
```
#### Zeige eine kurze Version an:
```shell
git status -s
```
#### Zeige nur verfolgte (getrackte) Dateien an:
```shell
git status --untracked-files=no
```
#### Zeige eine kurze Version mit zusätzlichen Informationen über den Branch an:
```shell
git status -sb
```
{% endraw %}