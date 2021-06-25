---
layout: default
title: "tex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tex">
  <a href="/de/common/tex.html">tex</a> <a href="#tex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kompiliere eine TeX Quelldatei in ein DVI Dokument.
> Weitere Informationen: <https://www.tug.org/begin.html>.

#### Kompiliere ein DVI Dokument:
```shell
tex {{quelldatei.tex}}
```
#### Kompiliere ein DVI Dokument und gib ein bestimmtes Output-Verzeichnis an:
```shell
tex -output-directory={{pfad/zu/verzeichnis}} {{quelldatei.tex}}
```
#### Kompiliere ein DVI Dokument und stoppe bei jedem Fehler:
```shell
tex -halt-on-error {{quelldatei.tex}}
```
{% endraw %}