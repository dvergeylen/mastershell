---
layout: default
title: "berks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="berks">
  <a href="/it/common/berks.html">berks</a> <a href="#berks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di dipendenze per Chef cookbooks.
> Maggiori informazioni: <https://docs.chef.io/berkshelf.html>.

#### Installa dipendenze cookbook in una repo locale:
```shell
berks install
```
#### Aggiorna uno specifico cookbook e le sue dipendenze:
```shell
berks update {{cookbook}}
```
#### Carica un cookbook sul server di Chef:
```shell
berks upload {{cookbook}}
```
#### Mostra le dipendenze di un cookbook:
```shell
berks contingent {{cookbook}}
```
{% endraw %}