---
layout: default
title: "git fsck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-fsck">
  <a href="/fr/common/git-fsck.html">git fsck</a> <a href="#git-fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vérifier la validité et la connectivité des nœuds dans un dépôt Git.
> N'applique aucune modification. Voir `git gc` pour nettoyer.
> Plus d'informations : <https://git-scm.com/docs/git-fsck>.

#### Vérifier le registre courant :
```shell
git fsck
```
#### Lister tous les tags trouvés :
```shell
git fsck --tags
```
#### Lister tout les nœuds racine trouvés :
```shell
git fsck --root
```
{% endraw %}