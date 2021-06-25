---
layout: default
title: "git sizer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-sizer">
  <a href="/it/common/git-sizer.html">git sizer</a> <a href="#git-sizer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calcola varie metriche dimensionali su repository Git e avvisa quando i loro valori rilevano problematicità.
> Maggiori informazioni: <https://github.com/github/git-sizer>.

#### Mostra solo le statistiche che hanno un livello di rischio maggiore di 0:
```shell
git sizer
```
#### Mostra tutte le statistiche:
```shell
git sizer -v
```
#### Mostra opzioni aggiuntive:
```shell
git sizer -h
```
{% endraw %}