---
layout: default
title: "netselect-apt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="netselect-apt">
  <a href="/en/linux/netselect-apt.html">netselect-apt</a> <a href="#netselect-apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a `sources.list` file for a Debian mirror with the lowest latency.
> More information: <https://manpages.debian.org/buster/netselect-apt/netselect-apt.1.html>.

#### Create `sources.list` using the lowest latency server:
```shell
sudo netselect-apt
```
#### Specify Debian branch, stable is used by default:
```shell
sudo netselect-apt {{testing}}
```
#### Include non-free section:
```shell
sudo netselect-apt --non-free
```
#### Specify a country for the mirror list lookup:
```shell
sudo netselect-apt -c {{India}}
```
{% endraw %}