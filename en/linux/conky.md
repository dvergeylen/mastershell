---
layout: default
title: "conky"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="conky">
  <a href="/en/linux/conky.html">conky</a> <a href="#conky"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Light-weight system monitor for X.
> More information: <https://github.com/brndnmtthws/conky>.

#### Launch with default, built-in config:
```shell
conky
```
#### Create a new default config:
```shell
conky -C > ~/.conkyrc
```
#### Launch conky with a given config file:
```shell
conky -c {{path/to/config}}
```
#### Start in the background (daemonize):
```shell
conky -d
```
#### Align conky on the desktop:
```shell
conky -a {{{top,bottom,middle}_{left,right,middle}}}
```
#### Pause for 5 seconds at startup before launching:
```shell
conky -p {{5}}
```
{% endraw %}