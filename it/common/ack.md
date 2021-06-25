---
layout: default
title: "ack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ack">
  <a href="/it/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un tool di ricerca simile a `grep`, ottimizzato per programmatori.
> Vedi anche: `rg`, che è molto più veloce.
> Maggiori informazioni: <https://beyondgrep.com/documentation/>.

#### Cerca ricorsivamente file contenenti una stringa o un'espressione regolare nella cartella corrente:
```shell
ack "{{pattern_di_ricerca}}"
```
#### Cerca un pattern in modalità case-insensitive:
```shell
ack --ignore-case "{{pattern_di_ricerca}}"
```
#### Cerca righe di testo contenenti un pattern, mostrando solo il testo corrispondente e non il resto della riga:
```shell
ack -o "{{pattern_di_ricerca}}"
```
#### Limita la ricerca ai file di un tipo specifico:
```shell
ack --type={{ruby}} "{{pattern_di_ricerca}}
```
#### Non cercare nei file di un tipo specifico:
```shell
ack --type=no{{ruby}} "{{pattern_di_ricerca}}
```
#### Conta il numero totale di corrispondenze trovate:
```shell
ack --count --no-filename "{{pattern_di_ricerca}}"
```
#### Mostra i nomi dei file e il numero di corrispondenze per ogni singolo file:
```shell
ack --count --files-with-matches "{{pattern_di_ricerca}}"
```
#### Mostra la lista di tutti i valori che possono essere usati con `--type`:
```shell
ack --help-types
```
{% endraw %}