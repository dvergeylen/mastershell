---
layout: default
title: "wormhole"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wormhole">
  <a href="/en/common/wormhole.html">wormhole</a> <a href="#wormhole"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get things from one computer to another, safely.
> More information: <https://magic-wormhole.readthedocs.io/en/latest/>.

#### Send a file:
```shell
wormhole send {{path/to/file}}
```
#### Receive a file:
```shell
wormhole receive {{wormhole_code}}
```
#### Send raw text:
```shell
wormhole send
```
{% endraw %}