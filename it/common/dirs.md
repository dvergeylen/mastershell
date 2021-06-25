---
layout: default
title: "dirs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dirs">
  <a href="/it/common/dirs.html">dirs</a> <a href="#dirs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra o manipola uno stack di directory.
> Uno stack di directory è una lista di directory recentemente visitate che può essere manipolata con i comandi `pushd` e `popd`.
> Maggiori informazioni: <https://www.gnu.org/software/bash/manual/bash.html#Directory-Stack-Builtins>.

#### Mostra lo stack di directory dividendo i nomi con uno spazio:
```shell
dirs
```
#### Mostra lo stack di directory una per riga:
```shell
dirs -p
```
#### Mostra solo l'ennesima directory dello stack (gli indici partono da 0):
```shell
dirs +{{N}}
```
#### Pulisci lo stack di directory:
```shell
dirs -c
```
{% endraw %}