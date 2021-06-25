---
layout: default
title: "env"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="env">
  <a href="/it/common/env.html">env</a> <a href="#env"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra le variabili d'ambiente o esegui un programma in un ambiente modificato.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/env>.

#### Mostra le variabili d'ambiente:
```shell
env
```
#### Esegui un programma. Utilizzato spesso in script dopo lo shebang (#!) per cercare il percorso del programma:
```shell
env {{programma}}
```
#### Resetta l'ambiente ed esegui un programma:
```shell
env -i {{programma}}
```
#### Rimuovi una variabile dall'ambiente ed esegui un programma:
```shell
env -u {{variabile}} {{programma}}
```
#### Setta una variabile ed esegui un programma:
```shell
env {{variabile}}={{valore}} {{programma}}
```
{% endraw %}