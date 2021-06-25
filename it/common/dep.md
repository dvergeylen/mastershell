---
layout: default
title: "dep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dep">
  <a href="/it/common/dep.html">dep</a> <a href="#dep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento di gestione delle dipendenze per progetti Go.
> Maggiori informazioni: <https://golang.github.io/dep>.

#### Inizializza la directory corrente come radice di un progetto Go:
```shell
dep init
```
#### Installa dipendenze mancanti (scannerizza `Gopkg.toml` ed i file `.go`):
```shell
dep ensure
```
#### Mostra lo stato delle dipendenze di un progetto:
```shell
dep status
```
#### Aggiungi una dipendenza al progetto:
```shell
dep ensure -add {{url_pacchetto}}
```
#### Aggiorna le versioni bloccate (in `Gopkg.lock`) di tutte le dipendenze:
```shell
dep ensure -update
```
{% endraw %}