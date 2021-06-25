---
layout: default
title: "var-dump-server"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="var-dump-server">
  <a href="/en/common/var-dump-server.html">var-dump-server</a> <a href="#var-dump-server"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Symfony dump server.
> Collects data dumped by the Symfony VarDumper component.
> More information: <https://symfony.com/doc/current/components/var_dumper.html#the-dump-server>.

#### Start the server:
```shell
var-dump-server
```
#### Dump the data in an HTML file:
```shell
var-dump-server --format=html > {{path/to/file.html}}
```
#### Make the server listen on a specific address and port:
```shell
var-dump-server --host {{127.0.0.1:9912}}
```
{% endraw %}