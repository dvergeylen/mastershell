---
layout: default
title: "which"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="which">
  <a href="/fr/common/which.html">which</a> <a href="#which"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Localise un programme dans le chemin de l'utilisateur.

#### Fouille la variable d'environnement « PATH » et affiche l'emplacement des programmes exécutables correspondants à la requête :
```shell
which {{exécutable}}
```
#### Affiche tous les exécutables correspondants à la requête, s'il y en a plus qu'un :
```shell
which -a {{exécutable}}
```
{% endraw %}