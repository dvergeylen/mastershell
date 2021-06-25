---
layout: default
title: "git instaweb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-instaweb">
  <a href="/en/common/git-instaweb.html">git instaweb</a> <a href="#git-instaweb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Helper to launch a gitweb server.
> More information: <https://git-scm.com/docs/git-instaweb>.

#### Launch a gitweb server for the current Git repository:
```shell
git instaweb --start
```
#### Listen only on localhost:
```shell
git instaweb --start --local
```
#### Listen on a specific port:
```shell
git instaweb --start --port {{1234}}
```
#### Use a specified http daemon:
```shell
git instaweb --start --httpd {{lighttpd|apache2|mongoose|plackup|webrick}}
```
#### Also auto-launch a web browser:
```shell
git instaweb --start --browser
```
#### Stop the currently running gitweb server:
```shell
git instaweb --stop
```
#### Restart the currently running gitweb server:
```shell
git instaweb --restart
```
{% endraw %}