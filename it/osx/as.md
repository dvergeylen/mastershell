---
layout: default
title: "as"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="as">
  <a href="/it/osx/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Assembler GNU portabile.
> Progettato principalmente per assemblare l'output di `gcc` ed utilizzarlo con `ld`.

#### Assembla un file, scrivendo l'output su a.out:
```shell
as {{file.s}}
```
#### Assembla l'output nel file dato:
```shell
as {{file.s}} -o {{out.o}}
```
#### Genera l'output più velocemente saltando gli spazi e senza preprocessare i commenti. (Questo comando dovrebbe essere utilizzato solo con compilatori fidati):
```shell
as -f {{file.s}}
```
#### Includi un percorso dato alla lista delle cartelle in cui cercare i file specificati nelle direttive `.include`:
```shell
as -I {{path/to/directory}} {{file.s}}
```
{% endraw %}