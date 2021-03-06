---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/it/linux/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copia file e cartelle.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/cp>.

#### Copia un file in un'altra posizione:
```shell
cp {{persorso/al/file_da_copiare.est}} {{percorso/al/file_di_destinazione.est}}
```
#### Copia un file all'interno di una cartella, mantenendone uguale il nome:
```shell
cp {{percorso/al/file_da_copiare.est}} {{percorso/alla/cartella}}
```
#### Copia ricorsivamente i contenuti di una cartella in un'altra posizione (se la destinazione esiste, la cartella è copiata al suo interno):
```shell
cp -r {{percorso/alla/cartella_da_copiare}} {{percorso/di/destinazione}}
```
#### Copia una cartella ricorsivamente in modalità prolissa (mostra i file mentre vengono copiati):
```shell
cp -vr {{percorso/alla/cartella_da_copiare}} {{percorso/di/destinazione}}
```
#### Copia i file di testo in un'altra posizione, in modalità interattiva (richiede conferma all'utente prima di sovrascrivere):
```shell
cp -i {{*.txt}} {{percorso/di/destinazione}}
```
#### Segue i collegamenti simbolici prima di copiare:
```shell
cp -L {{collegamento}} {{percorso/di/destinazione}}
```
#### Utilizza il percorso completo dei file originali, creando ogni cartella intermedia mancante mentre durante la copia:
```shell
cp --parents {{percorso/dei/file/da/copiare}} {{percorso/al/file/destinazione}}
```
{% endraw %}