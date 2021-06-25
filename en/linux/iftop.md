---
layout: default
title: "iftop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iftop">
  <a href="/en/linux/iftop.html">iftop</a> <a href="#iftop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show bandwidth usage on an interface by host.
> More information: <https://manned.org/iftop>.

#### Show the bandwidth usage:
```shell
sudo iftop
```
#### Show the bandwidth usage of a given interface:
```shell
sudo iftop -i {{interface}}
```
#### Show the bandwidth usage with port information:
```shell
sudo iftop -P
```
#### Do not show bar graphs of traffic:
```shell
sudo iftop -b
```
#### Do not look up hostnames:
```shell
sudo iftop -n
```
#### Get help about interactive commands:
```shell
?
```
{% endraw %}