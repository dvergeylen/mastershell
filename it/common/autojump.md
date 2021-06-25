---
layout: default
title: "autojump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autojump">
  <a href="/it/common/autojump.html">autojump</a> <a href="#autojump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Salta velocemente tra le directory che usi più spesso.
> Alias come j o jc sono disponibili per una maggiore velocità di scrittura.
> Maggiori informazioni: <https://github.com/wting/autojump>.

#### Muoviti in una directory il cui nome contiene una parola chiave:
```shell
j {{parola_chiave}}
```
#### Salta in una sotto-directory della directory corrente il quale nome contiene una parola chiave:
```shell
jc {{parola_chiave}}
```
#### Apri una directory il cui nome contiene una parola chiave nel gestore file di sistema:
```shell
jo {{parola_chiave}}
```
#### Rimuovi directory non esistenti dal database di autojump:
```shell
j --purge
```
#### Mostra le voci nel database di autojump:
```shell
j -s
```
{% endraw %}