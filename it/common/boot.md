---
layout: default
title: "boot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="boot">
  <a href="/it/common/boot.html">boot</a> <a href="#boot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumenti di build per il linguaggio di programmazione Clojure.
> Maggiori informazioni: <https://github.com/boot-clj/boot>.

#### Avvia una sessione REPL con il progetto o da sola:
```shell
boot repl
```
#### Builda un singolo `uberjar`:
```shell
boot jar
```
#### Mostra aiuto per un comando:
```shell
boot cljs --help
```
#### Genera le fondamenta per un nuovo progetto basandoti su una template:
```shell
boot --dependencies boot/new new --template {{nome_template}} --name {{nome_progetto}}
```
#### Builda per development (se si sta utilizzando il template boot/new):
```shell
boot dev
```
#### BUilda per produzione (se si sta utilizzando il template boot/new):
```shell
boot prod
```
{% endraw %}