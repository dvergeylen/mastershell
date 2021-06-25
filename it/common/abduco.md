---
layout: default
title: "abduco"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="abduco">
  <a href="/it/common/abduco.html">abduco</a> <a href="#abduco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di sessioni di terminale.
> Maggiori informazioni: <http://www.brain-dump.org/projects/abduco/>.

#### List sessioni:
```shell
abduco
```
#### Entra in una sessione, creandola se non esiste già:
```shell
abduco -A {{nome_sessione}} {{bash}}
```
#### Entra in una sessione con `dvtm`, creandola se non esiste già:
```shell
abduco -A {{nome_sessione}}
```
#### Esci da una sessione:
```shell
CTRL + \
```
#### Entra in una sessione in modalità sola lettura:
```shell
abduco -Ar {{nome_sessione}}
```
{% endraw %}