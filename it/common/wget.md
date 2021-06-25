---
layout: default
title: "wget"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wget">
  <a href="/it/common/wget.html">wget</a> <a href="#wget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scarica file dal Web.
> Supporta HTTP, HTTPS, FTP.
> Maggiori informazioni: <https://www.gnu.org/software/wget>.

#### Scarica il contenuto dell'URL in un file (dal nome "abcd" in questo caso):
```shell
wget {{https://esempio.com/abcd}}
```
#### Scarica il contenuto dell'URL in un file (dal nome "efgh" in questo caso):
```shell
wget --output-document {{efgh}} {{https://esempio.com/abcd}}
```
#### Scarica una singola pagina web e tutte le sue risorse (script, immagini, stili, ecc..) aspettando 3 secondi dopo ogni richiesta:
```shell
wget --page-requisites --convert-links --wait=3 {{https://esempio.com/pagina_web.html}}
```
#### Scarica tutti i file elencati nella cartella e nelle sue sotto-cartelle (non scarica gli elementi incorporati nella pagina):
```shell
wget --mirror --no-parent {{https://esempio.com/unqualchepercorso/}}
```
#### Limita la velocità di download e il numero di tentativi di connessione:
```shell
wget --limit-rate={{300k}} --tries={{100}} {{https://esempio.com/unqualchepercorso/}}
```
#### Scarica un file da un server HTTP trasmettendo le credenziali tramite Basis Auth (funzione anche con FTP):
```shell
wget --user={{nome_utente}} --password={{password}} {{https://esempio.com}}
```
#### Riprende un download incompleto:
```shell
wget --continue {{https://esempio.com}}
```
#### Scarica tutti gli URL contenuti in un file di testo in una cartella specificata:
```shell
wget --directory-prefix {{percorso/alla/cartella}} --input-file {{lista_di_URL.txt}}
```
{% endraw %}