---
layout: default
title: "grep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grep">
  <a href="/fr/common/grep.html">grep</a> <a href="#grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recherche des motifs dans un texte.
> Supporte des motifs simples et des expressions régulières.
> Plus d'informations : <https://www.gnu.org/software/grep/manual/grep.html>.

#### Recherche une chaîne de caractères précise :
```shell
grep {{chaîne_recherchée}} {{chemin/vers/fichier}}
```
#### Recherche en ignorant la casse :
```shell
grep -i {{chaîne_recherchée}} {{chemin/vers/fichier}}
```
#### Recherche récursivement (en ignorant les fichiers non-texte) dans le dossier courant une chaîne de caractères précise :
```shell
grep -RI {{chaîne_recherchée}} .
```
#### Utilise des expressions régulières étendues (supporte `?`, `+`, `{}`, `()` et `|`) :
```shell
grep -E {{expression_régulière}} {{chemin/vers/fichier}}
```
#### Affiche 3 lignes de [C]ontexte, avant ([B]efore), ou [A]près chaque concordance :
```shell
grep -{{C|B|A}} 3 {{chaîne_recherchée}} {{chemin/vers/fichier}}
```
#### Affiche le nom du fichier avec la ligne correspondante pour chaque concordance :
```shell
grep -Hn {{chaîne_recherchée}} {{chemin/vers/fichier}}
```
#### Utilise l'entrée standard au lieu d'un fichier :
```shell
cat {{chemin/vers/fichier}} | grep {{chaîne_recherchée}}
```
#### Inverse le résultat pour exclure des chaînes de caractères spécifiques :
```shell
grep -v {{chaîne_recherchée}}
```
{% endraw %}