---
layout: default
title: "xxd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xxd">
  <a href="/it/common/xxd.html">xxd</a> <a href="#xxd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra la rappresentazione esadecimale (hexdump) di un file binario e viceversa.

#### Creare l'hexdump di un file binario e mostrare l'output:
```shell
xxd {{file_di_input}}
```
#### Creare l'hexdump di un file binario e salvare il risultato in un file:
```shell
xxd {{file_di_input}} {{file_di_output}}
```
#### Mostrare un output in una versione un po' più compatta, dove gli zero consegutivi vengono sostituiti da un asterisco.
```shell
xxd -a {{file_di_input}}
```
#### Mostrare l'output in 10 colonne di un ottetto (byte) ciascuna:
```shell
xxd -c {{10}} {{file_di_input}}
```
#### Mostrare l'output solo fino ad una lunghezza massima di 32 bytes:
```shell
xxd -l {{32}} {{file_di_input}}
```
#### Mostrare l'output in modalità normale, senza spazi tra le colonne:
```shell
xxd -p {{file_di_input}}
```
#### Eseguire l'operazione inversa, ovvero da un hexdump creare il binario e salvarlo in un file:
```shell
xxd -r -p {{file_di_input}} {{file_di_output}}
```
{% endraw %}