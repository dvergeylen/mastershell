---
layout: default
title: "exec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exec">
  <a href="/it/common/exec.html">exec</a> <a href="#exec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sostituisci il processo corrente con un altro.

#### Sostituisci con il comando specificato utilizzando le variabili di ambiente correnti:
```shell
exec {{comando -con -flag}}
```
#### Sostituisci con il comando specificato utilizzando un ambiente vuoto:
```shell
exec -c {{comando -con -flag}}
```
#### Sostituisci con il comando specificato ed esegui il login con la shell predefinita:
```shell
exec -l {{comando -con -flag}}
```
#### Sostituisci con il comando specificato e cambia il nome del processo:
```shell
exec -a {{nuovo_nome_processo}} {{comando -con -flag}}
```
{% endraw %}