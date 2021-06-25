---
layout: default
title: "git pull"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-pull">
  <a href="/de/common/git-pull.html">git pull</a> <a href="#git-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Hole Branches von einem entfernten Repository und binde sie in das lokale Repository ein.
> Weitere Informationen: <https://git-scm.com/docs/git-pull>.

#### Lade Änderungen vom Standard-Repository herunter und führe diese zusammen:
```shell
git pull
```
#### Lade Änderungen vom Standard-Repository herunter und wende einen Rebase an:
```shell
git pull --rebase
```
#### Lade Änderungen vom Standard-Repository herunter und führe diese in den HEAD zusammen:
```shell
git pull {{remote_name}} {{branch}}
```
{% endraw %}