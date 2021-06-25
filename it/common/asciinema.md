---
layout: default
title: "asciinema"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asciinema">
  <a href="/it/common/asciinema.html">asciinema</a> <a href="#asciinema"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Registra e riproduci sessioni di terminale, condividendole opzionalmente su asciiname.org.
> Maggiori informazioni: <https://asciinema.org/>.

#### Associa l'installazione locale di `asciiname` ad un account di asciiname.org:
```shell
asciinema auth
```
#### Avvia una nuova registrazione (una volta terminata, verrà chiesto se caricarla o salvarla localmente):
```shell
asciinema rec
```
#### Avvia una nuova registrazione e salvala come file locale:
```shell
asciinema rec {{nome_registrazione}}.cast
```
#### Riproduci una sessione da un file locale:
```shell
asciinema play {{percorso/al/file}}.cast
```
#### Riproducei una sessione da asciinema.org:
```shell
asciinema play https://asciinema.org/a/{{id_registrazione}}
```
#### Avvia una nuova registrazione, limitando qualsiasi periodo di inattività a 2.5 secondi:
```shell
asciinema rec -i {{2.5}}
```
#### Stampa l'output completo di una sessione locale:
```shell
asciinema cat {{percorso/al/file}}.cast
```
#### Carica una sessione locale su asciinama.org:
```shell
asciinema upload {{percorso/al/file}}.cast
```
{% endraw %}