---
layout: default
title: "hg serve"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-serve">
  <a href="/en/common/hg-serve.html">hg serve</a> <a href="#hg-serve"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Start a standalone Mercurial web server for browsing repositories.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#serve>.

#### Start a web server instance:
```shell
hg serve
```
#### Start a web server instance on the specified port:
```shell
hg serve --port {{port}}
```
#### Start a web server instance on the specified listening address:
```shell
hg serve --address {{address}}
```
#### Start a web server instance with a specific identifier:
```shell
hg serve --name {{name}}
```
#### Start a web server instance using the specified theme (see the templates directory):
```shell
hg serve --style {{style}}
```
#### Start a web server instance using the specified SSL certificate bundle:
```shell
hg serve --certificate {{path/to/certificate}}
```
{% endraw %}