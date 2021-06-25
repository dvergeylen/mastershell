---
layout: default
title: "latex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="latex">
  <a href="/de/common/latex.html">latex</a> <a href="#latex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere eine LaTeX Quelldatei in ein DVI Dokument.
> Weitere Informationen: <https://www.latex-project.org>.

#### Kompiliere ein DVI Dokument:
```shell
latex {{quelldatei.tex}}
```
#### Kompiliere ein DVI Dokument und gib ein bestimmtes Output-Verzeichnis an:
```shell
latex -output-directory={{pfad/zu/verzeichnis}} {{quelldatei.tex}}
```
#### Kompiliere ein DVI Dokument und stoppe bei jedem Fehler:
```shell
latex -halt-on-error {{quelldatei.tex}}
```
{% endraw %}