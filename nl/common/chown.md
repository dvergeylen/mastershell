---
layout: default
title: "chown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chown">
  <a href="/nl/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verander gebruiker- en groepsbeheer van bestanden en mappen.
> Meer informatie: <https://www.gnu.org/software/coreutils/chown>.

#### Verander gebruikkersbeheerder van een bestand/map:
```shell
chown {{gebruiker}} {{pad/naar/bestand_of_map}}
```
#### Verander de gebruikersbeheerder en -groep van een bestand of map:
```shell
chown {{gebruiker}}:{{groep}} {{pad/naar/bestand_of_map}}
```
#### Verander recursief de beheerder van een map en alle inhoud:
```shell
chown -R {{gebruiker}} {{pad/naar/bestand_of_map}}
```
#### Verander de gebruiker van een symbolische link:
```shell
chown -h {{gebruiker}} {{pad/naar/symlink}}
```
#### Verander de beheerder van een bestand of map naar dezelfde als een referentiebestand:
```shell
chown --reference={{pad/naar/referentiebestand}} {{pad/naar/bestand_of_map}}
```
{% endraw %}