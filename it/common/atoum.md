---
layout: default
title: "atoum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atoum">
  <a href="/it/common/atoum.html">atoum</a> <a href="#atoum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un semplice, moderno ed intuitivo framework PHP per unit testing.
> Maggiori informazioni: <http://atoum.org>.

#### Inizializza un file di configurazione:
```shell
atoum --init
```
#### Esegui tutti i test:
```shell
atoum
```
#### Esegui test utilizzando uno specifico file di configurazione:
```shell
atoum -c {{percorso/al/file}}
```
#### Esegui uno specifico file di test:
```shell
atoum -f {{percorso/al/file}}
```
#### Esegui una specifica directory di test:
```shell
atoum -d {{path/to/directory}}
```
#### Esegui tutti i test sotto uno specifico namespace:
```shell
atoum -ns {{namespace}}
```
#### Esegui tutti i test con uno speficico tag:
```shell
atoum -t {{tag}}
```
#### Carica un file di bootstrap personalizzato prima di eseguire i test:
```shell
atoum --bootstrap-file {{percorso/al/file}}
```
{% endraw %}