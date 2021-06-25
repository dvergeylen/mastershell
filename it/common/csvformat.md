---
layout: default
title: "csvformat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvformat">
  <a href="/it/common/csvformat.html">csvformat</a> <a href="#csvformat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converti un file CSV in un formato di output personalizzato.
> Incluso in csvkit.
> Maggiori informazioni: <https://csvkit.readthedocs.io/en/latest/scripts/csvformat.html>.

#### Converti in un file delimitato da tab (TSV):
```shell
csvformat -T {{dati.csv}}
```
#### Converti i delimitatori in un carattere personalizzato:
```shell
csvformat -D "{{carattere_personalizzato}}" {{dati.csv}}
```
#### Converti caratteri newline a carriage return (^M) + newline:
```shell
csvformat -M "{{\r\n}}" {{dati.csv}}
```
#### Minimizza l'utilizzo delle virgolette:
```shell
csvformat -U 0 {{dati.csv}}
```
#### Massimizza l'utilizzo delle virgolette:
```shell
csvformat -U 1 {{dati.csv}}
```
{% endraw %}