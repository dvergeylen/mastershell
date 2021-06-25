---
layout: default
title: "cake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cake">
  <a href="/en/common/cake.html">cake</a> <a href="#cake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The command-line processor for the CakePHP framework.
> More information: <https://cakephp.org>.

#### Display basic information about the current app and available commands:
```shell
cake
```
#### Display a list of available routes:
```shell
cake routes
```
#### Clear configuration caches:
```shell
cake cache clear_all
```
#### Build the metadata cache:
```shell
cake schema_cache build --connection {{connection}}
```
#### Clear the metadata cache:
```shell
cake schema_cache clear
```
#### Clear a single cache table:
```shell
cake schema_cache clear {{table_name}}
```
#### Start a development web server (defaults to port 8765):
```shell
cake server
```
#### Start a REPL interactive shell instance:
```shell
cake console
```
{% endraw %}