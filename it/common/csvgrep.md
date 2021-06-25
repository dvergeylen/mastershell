---
layout: default
title: "csvgrep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvgrep">
  <a href="/it/common/csvgrep.html">csvgrep</a> <a href="#csvgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Filtra righe CSV con stringhe e pattern matching.
> Incluso in csvkit.
> Maggiori informazioni: <https://csvkit.readthedocs.io/en/latest/scripts/csvgrep.html>.

#### Trova righe contenenti una certa stringa nella colonna 1:
```shell
csvgrep -c {{1}} -m {{stringa}} {{data.csv}}
```
#### Trova righe per le quali le colonne 3 e 4 soddisfano una certa espressione regolare:
```shell
csvgrep -c {{3,4}} -r {{espressione_regolare}} {{data.csv}}
```
#### Trova righe dove la colonna "nome" NON include la stringa "Mario Rossi":
```shell
csvgrep -i -c {{nome}} -m "{{Mario Rossi}}" {{data.csv}}
```
{% endraw %}