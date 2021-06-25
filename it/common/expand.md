---
layout: default
title: "expand"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="expand">
  <a href="/it/common/expand.html">expand</a> <a href="#expand"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converti caratteri tab in spazi.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/expand>.

#### Converti tab in un file in spazi, scrivendo su standard output:
```shell
expand {{file}}
```
#### Converti i tab in spazi, leggendo da standard input:
```shell
expand
```
#### Non convertire i tab dopo caratteri di spaziatura:
```shell
expand -i {{file}}
```
#### Sostituisci i tab con un determinato numeroo di spazi, non 8 (default):
```shell
expand -t={{numero_spazi}} {{file}}
```
#### Utilizza una lista separata da virgole di posizioni esplicite di tab:
```shell
expand -t={{1,4,6}}
```
{% endraw %}