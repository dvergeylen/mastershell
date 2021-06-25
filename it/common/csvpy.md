---
layout: default
title: "csvpy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvpy">
  <a href="/it/common/csvpy.html">csvpy</a> <a href="#csvpy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Carica un file CSV in una shell Python.
> Incluso in csvkit.
> Maggiori informazioni: <https://csvkit.readthedocs.io/en/latest/scripts/csvpy.html>.

#### Carica un file CSV in un oggetto `CSVKitReader`:
```shell
csvpy {{data.csv}}
```
#### Carica un file CSV in un oggetto `CSVKitDictReader`:
```shell
csvpy --dict {{data.csv}}
```
{% endraw %}