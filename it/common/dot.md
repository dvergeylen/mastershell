---
layout: default
title: "dot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dot">
  <a href="/it/common/dot.html">dot</a> <a href="#dot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento da linea di comando per produrre disegni a livelli di grafi orientati.
> Maggiori informazioni: <https://www.graphviz.org/pdf/dotguide.pdf>.

#### Renderizza un'immagine determinando il nome del file di output dal nome del file di input ed il formato:
```shell
dot -Tpng -O {{percorso/al/file.dot}}
```
#### Crea una SVG da un file DOT:
```shell
dot -Tsvg -o {{percorso/al/file_output.svg}} {{percorso/al/file.dot}}
```
{% endraw %}