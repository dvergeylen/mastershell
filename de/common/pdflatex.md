---
layout: default
title: "pdflatex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdflatex">
  <a href="/de/common/pdflatex.html">pdflatex</a> <a href="#pdflatex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere eine LaTeX Quelldatei in ein PDF Dokument.
> Weitere Informationen: <https://manned.org/pdflatex>.

#### Kompiliere ein PDF Dokument:
```shell
pdflatex {{quelldatei.tex}}
```
#### Kompiliere ein PDF Dokument und gib ein bestimmtes Output-Verzeichnis an:
```shell
pdflatex -output-directory={{pfad/zu/verzeichnis}} {{quelldatei.tex}}
```
#### Kompiliere ein PDF Dokument und stoppe bei jedem Fehler:
```shell
pdflatex -halt-on-error {{quelldatei.tex}}
```
{% endraw %}