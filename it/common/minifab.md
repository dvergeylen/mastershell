---
layout: default
title: "minifab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="minifab">
  <a href="/it/common/minifab.html">minifab</a> <a href="#minifab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per semplificare il settaggio e il deployment di una blockchain Hyperledger Fabric.
> Maggiori informazioni: <https://github.com/hyperledger-labs/minifabric>.

#### Crea la blockchain Hyperledger Fabric:
```shell
minifab up -i {{versione_minifab}}
```
#### Rimuovi la blockchain Hyperledger Fabric:
```shell
minifab down
```
#### Installa smart contract su un canale:
```shell
minifab install -n {{nome_smart_contract}}
```
#### Installa smart contract su un canale specificando la versione:
```shell
minifab install -n {{nome_smart_contract}} -v {{versione_smart_contract}}
```
#### Inizializza smart contract dopo installazione/aggiornamento dello stesso:
```shell
minifab approve,commit,initialize,discover
```
#### Interroga smart contract con argomenti:
```shell
minifab invoke -n {{nome_smart_contract}} -p '"{{nome_metodo}}", "{{arg0}}", "{{arg1}}", ...'
```
#### Interroga la blockchain:
```shell
minifab blockquery {{numero_blocco}}
```
#### Esegui direttamente l'applicazione:
```shell
minifab apprun -l {{linguaggio_di_programmazione}}
```
{% endraw %}