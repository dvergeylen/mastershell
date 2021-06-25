---
layout: default
title: "exa"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exa">
  <a href="/it/common/exa.html">exa</a> <a href="#exa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un moderno sostituto per `ls` (elenca i contenuti di una directory).
> Maggiori informazioni: <https://the.exa.website>.

#### Elenca i file nella directory corrente, uno per riga:
```shell
exa --oneline
```
#### Elenca tutti i file, inclusi quelli nascosti:
```shell
exa --all
```
#### Elenca tutti i file e mostra informazioni (permessi, dimensione e data di ultima modifica):
```shell
exa --long --all
```
#### Elenca i file, ordinandoli per dimensione decrescente:
```shell
exa --reverse --sort={{size}}
```
#### Mostra un albero dei file con 3 livelli di profondità:
```shell
exa --long --tree --level={{3}}
```
#### Elenca i file e mostra informazioni, ordinandoli per ultima modifica (più vechci prima):
```shell
exa --long --sort={{modified}}
```
{% endraw %}