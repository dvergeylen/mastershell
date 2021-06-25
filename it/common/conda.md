---
layout: default
title: "conda"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="conda">
  <a href="/it/common/conda.html">conda</a> <a href="#conda"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestione pacchetti, dipendenze ed ambiente per qualsiasi linguaggio di programmazione.
> Maggiori informazioni: <https://github.com/conda/conda>.

#### Crea un nuovo ambiente, installandovi alcuni pacchetti:
```shell
conda create --name {{nome_ambiente}} {{python=2.7 matplotlib}}
```
#### Elenca tutti gli ambienti:
```shell
conda info --envs
```
#### Attiva o disattiva un ambiente:
```shell
conda {{activate|deactivate}} {{nome_ambiente}}
```
#### Elimina un ambiente rimuovendo anche tutti i pacchetti:
```shell
conda remove --name {{nome_ambiente}} --all
```
#### Cerca un determinato pacchetto nei canali di conda:
```shell
conda search {{package_name}}
```
#### Installa pacchetti nell'ambiente corrente:
```shell
conda install {{python=3.4 numpy}}
```
#### Elenca i pacchetti attualmente installati nell'ambiente corrente:
```shell
conda list
```
#### Elimina pacchetti inutilizzati e cache:
```shell
conda clean --all
```
{% endraw %}