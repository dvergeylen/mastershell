---
layout: default
title: "drush"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="drush">
  <a href="/it/common/drush.html">drush</a> <a href="#drush"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shell da linea di comando ed interfaccia di scripting per Drupal.
> Maggiori informazioni: <https://www.drush.org>.

#### Scarica il modulo "foo":
```shell
drush dl {{foo}}
```
#### Scarica la versione 7.x-2.1-beta1 del modulo "foo":
```shell
drush dl {{foo}}-7.x-2.1-beta1
```
#### Abilita il modulo "foo":
```shell
drush en {{foo}}
```
#### Disabilita il modulo "foo":
```shell
drush dis {{foo}}
```
#### Pulisci tutte le cache:
```shell
drush cc all
```
#### Pulisci le cache CSS e JavaScript:
```shell
drush cc css-js
```
{% endraw %}