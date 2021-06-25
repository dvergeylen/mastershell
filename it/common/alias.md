---
layout: default
title: "alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alias">
  <a href="/it/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea alias -- parole che sono sostituite da stringhe di comandi.
> Gli alias vengono persi alla chiusura della shell corrente, a meno che non siano definiti nel file di configurazione della shell (ad esempio `~/.bashrc`).
> Maggiori informazioni: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Crea un alias:
```shell
alias {{parola}}="{{comando}}"
```
#### Mostra il comando associato ad un dato alias:
```shell
alias {{parola}}
```
#### Rimuovi un alias:
```shell
unalias {{parola}}
```
#### Elenca tutti gli alias correntemente in uso:
```shell
alias -p
```
#### Rendi il comando rm interattivo:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Crea un alias `la` come scorciatoia per il comando `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}