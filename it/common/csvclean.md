---
layout: default
title: "csvclean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvclean">
  <a href="/it/common/csvclean.html">csvclean</a> <a href="#csvclean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trova e corregge errori di sintassi comuni in file CSV.
> Incluso in csvkit.
> Maggiori informazioni: <https://csvkit.readthedocs.io/en/latest/scripts/csvclean.html>.

#### Correggi un file CSV:
```shell
csvclean {{file.csv}}
```
#### Elenca le posizioni di errori di sintassi in un file CSV:
```shell
csvclean -n {{file.csv}}
```
{% endraw %}