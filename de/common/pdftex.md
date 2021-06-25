---
layout: default
title: "pdftex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdftex">
  <a href="/de/common/pdftex.html">pdftex</a> <a href="#pdftex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere eine TeX Quelldatei in ein PDF Dokument.
> Weitere Informationen: <https://www.tug.org/applications/pdftex/>.

#### Kompiliere ein PDF Dokument:
```shell
pdftex {{quelldatei.tex}}
```
#### Kompiliere ein PDF Dokument und gib ein bestimmtes Output-Verzeichnis an:
```shell
pdftex -output-directory={{pfad/zu/verzeichnis}} {{quelldatei.tex}}
```
#### Kompiliere ein PDF Dokument und stoppe bei jedem Fehler:
```shell
pdftex -halt-on-error {{quelldatei.tex}}
```
{% endraw %}