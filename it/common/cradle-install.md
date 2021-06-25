---
layout: default
title: "cradle install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-install">
  <a href="/it/common/cradle-install.html">cradle install</a> <a href="#cradle-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Installa i componenti del framework Cradle per PHP.
> Maggiori informazioni: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#install>.

#### Installa i componenti di Cradle (maggiori dettagli verranno richiesti all'utente):
```shell
cradle install
```
#### Sovrascrivi i file forzatamente:
```shell
cradle install --force
```
#### Salta l'esecuzione di migrazioni SQL:
```shell
cradle install --skip-sql
```
#### Salta l'esecuzione di aggiornamenti dei pacchetti:
```shell
cradle install --skip-versioning
```
#### Utilizza specifici dettagli per il database:
```shell
cradle install -h {{hostname}} -u {{nome_utente}} -p {{password}}
```
{% endraw %}