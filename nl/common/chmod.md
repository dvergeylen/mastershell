---
layout: default
title: "chmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chmod">
  <a href="/nl/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verander de toegangstoestemmingen van een bestand of map.
> Meer informatie: <https://www.gnu.org/software/coreutils/chmod>.

#### Geef een gebruiker ([u]ser) die het bestand beheert het recht om deze uit te voeren (e[x]ecute):
```shell
chmod u+x {{bestand}}
```
#### Geef de gebruiker ([u]ser) het recht om een bestand of map te lezen ([r]ead) en schrijven ([w]rite):
```shell
chmod u+rw {{bestand_of_map}}
```
#### Haal uitvoertoestemming (e[x]ecute) voor een bestand weg van de [g]roep:
```shell
chmod g-x {{bestand}}
```
#### Geef [a]lle gebruikers toegang om een bestand te lezen ([r]ead) en schrijven ([w]rite):
```shell
chmod a+rx {{bestand}}
```
#### Geef anderen ([o]thers) die niet in de groep van de beheerder zitten, dezelfde rechten als de [g]roep:
```shell
chmod o=g {{bestand}}
```
#### Haal alle rechten van de anderen ([o]thers) weg:
```shell
chmod o= {{bestand}}
```
#### Verander de toestemmingen recursief, waarbij de [g]roep en anderen ([o]thers) de mogelijkheid tot schrijven ([w]rite) krijgen:
```shell
chmod -R g+w,o+w {{map}}
```
{% endraw %}