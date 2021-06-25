---
layout: default
title: "git rev-parse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rev-parse">
  <a href="/fr/common/git-rev-parse.html">git rev-parse</a> <a href="#git-rev-parse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Afficher les métadonnées liées à des révisions spécifiques.
> Plus d'informations : <https://git-scm.com/docs/git-rev-parse>.

#### Afficher l'empreinte du commit de la branche courante :
```shell
git rev-parse {{nom_de_branche}}
```
#### Affiche le nom de la branche courante :
```shell
git rev-parse --abbrev-ref {{HEAD}}
```
#### Obtenir le chemin absolu du répertoire racine :
```shell
git rev-parse --show-toplevel
```
{% endraw %}