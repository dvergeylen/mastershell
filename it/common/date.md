---
layout: default
title: "date"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="date">
  <a href="/it/common/date.html">date</a> <a href="#date"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imposta o mostra data e ora di sistema.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/date>.

#### Mostra la data corrente utilizzando il formato predefinito della locale corrente:
```shell
date +"%c"
```
#### Mostra la data corrente in UTC e formato ISO 8601:
```shell
date -u +"%Y-%m-%dT%H:%M:%SZ"
```
#### Mostra la data corrente come timestamp Unix (secondi dall'epoca Unix):
```shell
date +%s
```
#### Mostra una specifica data (rappresentata come timestamp Unix) utilizzando il formato predefinito:
```shell
date -d @1473305798
```
#### Converti una specifica data in un timestamp Unix:
```shell
date -d "{{2018-09-01 00:00}}" +%s --utc
```
{% endraw %}