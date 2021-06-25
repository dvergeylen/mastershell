---
layout: default
title: "jest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jest">
  <a href="/fr/common/jest.html">jest</a> <a href="#jest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Une plateforme de test JavaScript sans configuration.
> Plus d'informations : <https://jestjs.io>.

#### Exécuter tous les tests disponibles :
```shell
jest
```
#### Exécuter les suites de test de fichiers donnés :
```shell
jest {{chemin/vers/fichier1}} {{chemin/vers/fichier2}}
```
#### Exécuter les suites de test pour des fichiers, dans le répertoire courant et ses sous-répertoires, dont le chemin correspond à l'expression régulière indiquée :
```shell
jest {{expression_régulière}} {{expression_régulière}}
```
#### Exécuter les tests dont les noms correspondent aux expressions régulières indiquées :
```shell
jest --testNamePattern {{nom_test}}
```
#### Exécuter les suites de test associées à un fichier source donné :
```shell
jest --findRelatedTests {{chemin/vers/fichier_source.js}}
```
#### Exécuter les suites de test associées à tous les fichiers non commités :
```shell
jest --onlyChanged
```
#### Surveiller les changements sur les fichiers et ré-exécuter les tests associés :
```shell
jest --watch
```
#### Montrer l'aide :
```shell
jest --help
```
{% endraw %}