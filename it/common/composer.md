---
layout: default
title: "composer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="composer">
  <a href="/it/common/composer.html">composer</a> <a href="#composer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un gestore di dipendenze a pacchetti per progetti PHP.
> Maggiori informazioni: <https://getcomposer.org/>.

#### Aggiungi un pacchetto come dipendenza per questo progetto, aggiungendolo a `composer.json`:
```shell
composer require {{user/nome_pacchetto}}
```
#### Installa tutte le dipendenze listate nel `composer.json` di questo progetto:
```shell
composer install
```
#### Disinstalla un pacchetto da questo progetto, rimuovendolo come dipendenza da `composer.json`:
```shell
composer remove {{user/nome_pacchetto}}
```
#### Aaggiorna tutte le dipendenze nel `composer.json` di questo progetto:
```shell
composer update
```
#### Aggiorna composer alla versione più recente:
```shell
composer self-update
```
{% endraw %}