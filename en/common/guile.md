---
layout: default
title: "guile"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="guile">
  <a href="/en/common/guile.html">guile</a> <a href="#guile"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Guile Scheme interpreter.
> More information: <https://www.gnu.org/software/guile>.

#### Start the Guile Scheme REPL:
```shell
guile
```
#### Execute the script in a given Scheme file:
```shell
guile {{script.scm}}
```
#### Execute a Scheme expression:
```shell
guile -c "{{expression}}"
```
#### Listen on a port or a Unix domain socket (the default is port 37146) for remote REPL connections:
```shell
guile --listen={{port_or_socket}}
```
{% endraw %}