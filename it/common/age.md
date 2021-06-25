---
layout: default
title: "age"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="age">
  <a href="/it/common/age.html">age</a> <a href="#age"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uno strumento semplice, moderno e sicuro per la cifratura di file.
> Maggiori informazioni: <https://age-encryption.org>.

#### Generare un file cifrato che può essere decifrato con una passphrase:
```shell
age --passphrase --output {{percorso/del/file_cifrato}} {{percorso/del/file_non_cifrato}}
```
#### Generare una coppia di chiavi, salvando la chiave privata in un file non cifrato e stampando sullo stdout la chiave pubblica:
```shell
age-keygen --output {{percorso/del/file}}
```
#### Cifrare un file con una o più chiavi pubbliche inserite come letterali:
```shell
age --recipient {{chiave_pubblica_1}} --recipient {{chiave_pubblica_2}} {{percorso/del/file_non_cifrato}} --output {{percorso/del/file_cifrato}}
```
#### Cifrare un file con una o più chiavi pubbliche specificate in un file di destinatari:
```shell
age --recipients-file {{percorso/del/file_di_destinatari}} {{percorso/del/file_non_cifrato}} --output {{percorso/del/file_cifrato}}
```
#### Decifrare un file con una passphrase:
```shell
age --decrypt --output {{percorso/del/file_decifrato}} {{percorso/del/file_cifrato}}
```
#### Decifrare un file con il file di una chiave privata:
```shell
age --decrypt --identity {{percorso/del/file_chiave_privata}} --output {{percorso/del/file_decifrato}} {{percorso/del/file_cifrato}}
```
{% endraw %}