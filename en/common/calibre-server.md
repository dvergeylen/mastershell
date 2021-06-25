---
layout: default
title: "calibre-server"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="calibre-server">
  <a href="/en/common/calibre-server.html">calibre-server</a> <a href="#calibre-server"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A server application that can be used to distribute e-books over a network.
> Note: e-books must already be imported into the library using the GUI or the `calibredb` CLI.
> More information: <https://manual.calibre-ebook.com/generated/en/calibre-server.html>.

#### Start a server to distribute e-books. Access at http://localhost:8080:
```shell
calibre-server
```
#### Start server on different port. Access at http://localhost:port:
```shell
calibre-server --port {{port}}
```
#### Password protect the server:
```shell
calibre-server --username {{username}} --password {{password}}
```
{% endraw %}