---
layout: default
title: "envsubst"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="envsubst">
  <a href="/it/common/envsubst.html">envsubst</a> <a href="#envsubst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sostituisci variabili di ambiente con il loro valore in stringhe di formato della shell.
> Le variabili da sostituire devono essere nella forma `${var}` oppure `$var`.
> Maggiori informazioni: <https://www.gnu.org/software/gettext/manual/html_node/envsubst-Invocation.html>.

#### Sostituisci variabili di ambiente in stdin e stampa l'output su stdout:
```shell
echo '{{$HOME}}' | envsubst
```
#### Sostituisci variabili di ambiente in un file input e stampa l'output su stdout:
```shell
envsubst < {{percorso/a/file_input}}
```
#### Sostituisci variabili di ambiente in un file input e scrivi l'output su un file:
```shell
envsubst < {{percorso/a/file_input}} > {{percorso/a/file_output}}
```
#### Sostituisci in un file input le variabili di ambiente specificate in una lista separata da spazi:
```shell
envsubst {{$USER $HOME $SHELL}} < {{percorso/a/file_input}}
```
{% endraw %}