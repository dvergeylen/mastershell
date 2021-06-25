---
layout: default
title: "git blame"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-blame">
  <a href="/de/common/git-blame.html">git blame</a> <a href="#git-blame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige den Commit-Hash und den letzten Autor jeder Zeile einer Datei.
> Weitere Informationen: <https://git-scm.com/docs/git-blame>.

#### Gib die Commit-Hashes und dem Autor jeder Zeile einer Datei aus:
```shell
git blame {{pfad/zu/datei}}
```
#### Gib die Commit-Hashes und dem Autor (inklusive Email) jeder Zeile einer Datei aus:
```shell
git blame -e {{pfad/zu/datei}}
```
{% endraw %}