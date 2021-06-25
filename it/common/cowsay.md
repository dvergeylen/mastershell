---
layout: default
title: "cowsay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cowsay">
  <a href="/it/common/cowsay.html">cowsay</a> <a href="#cowsay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Genera un personaggio ASCII (di default una mucca) che dice o pensa qualcosa.
> Maggiori informazioni: <https://github.com/tnalpgge/rank-amateur-cowsay>.

#### Stampa una mucca ASCII che dice "Hello world":
```shell
cowsay "Hello world"
```
#### Usa il testo da standard input per il fumetto:
```shell
echo "Ciao" | cowsay
```
#### Elenca tutti i personaggi disponibili:
```shell
cowsay -l
```
#### Stampa un drago ASCII che dice "Ciao":
```shell
cowsay -f dragon "Ciao"
```
#### Stampa una mucca ASCII sballata che pensa:
```shell
cowthink -s "Sono solo una mucca, non un grande pensatore..."
```
{% endraw %}