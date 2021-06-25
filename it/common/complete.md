---
layout: default
title: "complete"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="complete">
  <a href="/it/common/complete.html">complete</a> <a href="#complete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fornisce autocompletamento per argomenti dei comandi della shell.
> Maggiori informazioni: <https://www.gnu.org/software/bash/manual/html_node/Programmable-Completion-Builtins.html>.

#### Applica ad un comando una funzione per gestirne l'autocompletamento:
```shell
complete -F {{funzione}} {{comando}}
```
#### Applica ad un comando un altro comando per gestirne l'autocompletamento:
```shell
complete -C {{comando_per_autocompletamento}} {{comando}}
```
#### Applica l'autocompletamento senza aggiungere uno spazio dopo la parola completata:
```shell
complete -o nospace -F {{function}} {{comando}}
```
{% endraw %}