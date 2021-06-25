---
layout: default
title: "texliveonfly"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="texliveonfly">
  <a href="/de/common/texliveonfly.html">texliveonfly</a> <a href="#texliveonfly"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lade fehlende TeX Live Packages während dem Kompilieren einer `.tex` Datei herunter.
> Weitere Informationen: <https://ctan.org/pkg/texliveonfly>.

#### Lade fehlende Packages während dem Kompilieren herunter:
```shell
texliveonfly {{quelldatei.tex}}
```
#### Verwende einen bestimmten Compiler (standardmäßig `pdflatex`):
```shell
texliveonfly --compiler={{compiler}} {{quelldatei.tex}}
```
#### Verwende ein bestimmtes Tex Live `bin` Verzeichnis:
```shell
texliveonfly --texlive_bin={{pfad/zu/texlive_bin}} {{quelldatei.tex}}
```
{% endraw %}