---
layout: default
title: "ln"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ln">
  <a href="/fr/common/ln.html">ln</a> <a href="#ln"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crée des liens vers des fichiers et répertoires.
> Plus d'informations : <https://www.gnu.org/software/coreutils/ln>.

#### Crée un lien symbolique vers un fichier ou un répertoire :
```shell
ln -s {{/chemin/vers/fichier_ou_repertoire}} {{chemin/vers/lien_symbolique}}
```
#### Modifie la cible d'un lien symbolique existant :
```shell
ln -sf {{/chemin/vers/nouveau_fichier}} {{chemin/vers/lien_symbolique}}
```
#### Crée un lien dur vers un fichier :
```shell
ln {{/chemin/vers/fichier}} {{chemin/vers/lien_dur}}
```
{% endraw %}