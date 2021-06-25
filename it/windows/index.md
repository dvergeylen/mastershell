---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#cmd">cmd</a>

{% raw %}
<h2 id="cmd">
  <a href="/it/windows/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> L'interprete dei comandi di Windows.
> Maggiori informazioni: <https://docs.microsoft.com/it-it/windows-server/administration/windows-commands/cmd>.

#### Lancia una nuova istanza dell'interprete dei comandi:
```shell
cmd
```
#### Esegue il comando specificato e poi esce:
```shell
cmd /c "{{comando}}"
```
#### Esegue il comando specificato e poi apre una shell interattiva:
```shell
cmd /k "{{comando}}"
```
#### Disabilita l'uso di `echo` nell'output di un comando:
```shell
cmd /q
```
#### Abilita o disabilita le estensioni ai comandi:
```shell
cmd /e:{{on|off}}
```
#### Abilita o disabilita l'autocompletamento dei nomi di file e cartelle:
```shell
cmd /f:{{on|off}}
```
#### Abilita o disabilita l'espansione delle variabili d'ambiente:
```shell
cmd /v:{{on|off}}
```
#### Forza l'encoding delle stringhe in Unicode per l'output:
```shell
cmd /u
```
{% endraw %}