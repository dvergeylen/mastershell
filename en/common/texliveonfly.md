---
layout: default
title: "texliveonfly"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="texliveonfly">
  <a href="/en/common/texliveonfly.html">texliveonfly</a> <a href="#texliveonfly"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Downloads missing TeX Live packages while compiling `.tex` files.
> More information: <https://ctan.org/pkg/texliveonfly>.

#### Download missing packages while compiling:
```shell
texliveonfly {{source.tex}}
```
#### Use a specific compiler (defaults to `pdflatex`):
```shell
texliveonfly --compiler={{compiler}} {{source.tex}}
```
#### Use a custom TeX Live `bin` folder:
```shell
texliveonfly --texlive_bin={{path/to/texlive_bin}} {{source.tex}}
```
{% endraw %}