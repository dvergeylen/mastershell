---
layout: default
title: "git instaweb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-instaweb">
  <a href="/it/common/git-instaweb.html">git instaweb</a> <a href="#git-instaweb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Helper per avviare un server gitweb.
> Maggiori informazioni: <https://git-scm.com/docs/git-instaweb>.

#### Avvia un server gitweb dal repository corrente:
```shell
git instaweb --start
```
#### Resta in ascolto solo su localhost:
```shell
git instaweb --start --local
```
#### Resta in ascolto su una porta specifica:
```shell
git instaweb --start --port {{1234}}
```
#### Usa un http daemon specifico:
```shell
git instaweb --start --httpd {{lighttpd|apache2|mongoose|plackup|webrick}}
```
#### Avvia automaticamente anche un web browser:
```shell
git instaweb --start --browser
```
#### Interrompi il server gitweb in esecuzione:
```shell
git instaweb --stop
```
#### Riavvia il server gitweb in esecuzione:
```shell
git instaweb --restart
```
{% endraw %}