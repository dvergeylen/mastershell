---
layout: default
title: "git blame"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-blame">
  <a href="/fr/common/git-blame.html">git blame</a> <a href="#git-blame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche le hash de commit et le dernier auteur de chaque ligne d un fichier.
> Plus d'informations : <https://git-scm.com/docs/git-blame>.

#### Affiche le hash de commit et le nom de l auteur en face de chaque ligne :
```shell
git blame {{file}}
```
#### Affiche le hash de commit le nom et l email de l auteur en face de chaque ligne :
```shell
git blame -e {{file}}
```
{% endraw %}