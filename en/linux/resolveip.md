---
layout: default
title: "resolveip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="resolveip">
  <a href="/en/linux/resolveip.html">resolveip</a> <a href="#resolveip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Resolve hostnames to their IP addresses and vice versa.
> More information: <https://mariadb.com/kb/en/resolveip/>.

#### Resolve a hostname to an IP address:
```shell
resolveip {{example.org}}
```
#### Resolve an IP address to a hostname:
```shell
resolveip {{1.1.1.1}}
```
#### Silent mode. Produces less output:
```shell
resolveip --silent {{example.org}}
```
{% endraw %}