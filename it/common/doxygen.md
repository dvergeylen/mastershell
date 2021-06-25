---
layout: default
title: "doxygen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="doxygen">
  <a href="/it/common/doxygen.html">doxygen</a> <a href="#doxygen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un sistema di documentazione per diversi linguaggi di programmazione.
> Maggiori informazioni: <http://www.doxygen.nl>.

#### Genera il modello di configurazione di default `Doxyfile`:
```shell
doxygen -g
```
#### Genera un modello di file di configurazione:
```shell
doxygen -g {{percorso/a/file_config}}
```
#### Genera la documentazione utilizzando un file di configurazione esistente:
```shell
doxygen {{percorso/a/file_config}}
```
{% endraw %}