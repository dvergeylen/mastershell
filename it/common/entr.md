---
layout: default
title: "entr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="entr">
  <a href="/it/common/entr.html">entr</a> <a href="#entr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui comandi arbitrari al cambiamento di file.
> Maggiori informazioni: <https://manned.org/entr>.

#### Ricompila con `make` se qualsiasi file in quasiasi sottodirectory cambia:
```shell
{{ag -l}} | entr {{make}}
```
#### Ricompila e testa con `make` se qualsiasi file sorgente `.c` nella cartella corrente cambia:
```shell
{{ls *.c}} | entr {{'make && make test'}}
```
#### Invia il segnale `SIGTERM` ad un sottoprocesso ruby precedentemente avviato prima di eseguire `ruby main.rb`:
```shell
{{ls *.rb}} | entr -r {{ruby main.rb}}
```
#### Esegui un comando con il file cambiato (`/_`) come argomento:
```shell
{{ls *.sql}} | entr {{psql -f}} /_
```
{% endraw %}