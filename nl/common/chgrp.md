---
layout: default
title: "chgrp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chgrp">
  <a href="/nl/common/chgrp.html">chgrp</a> <a href="#chgrp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verander beheerdersgroep van bestanden en mappen.
> Meer informatie: <https://www.gnu.org/software/coreutils/chgrp>.

#### Verander beheerdergroep van een bestand of map:
```shell
chgrp {{groep}} {{pad/naar/bestand_of_map}}
```
#### Verander recursief de beheerdersgroep van een map en alle bestanden erin:
```shell
chgrp -R {{groep}} {{pad/naar/map}}
```
#### Verander beheerdersgroep van een symbolische link:
```shell
chgrp -h {{groep}} {{pad/naar/symlink}}
```
#### Verander de beheerdersgroep van een bestand/map naar de permissies van een referentiebestand:
```shell
chgrp --reference={{pad/naar/referentiebestand}} {{pad/naar/bestand_of_map}}
```
{% endraw %}