---
layout: default
title: "sic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sic">
  <a href="/en/linux/sic.html">sic</a> <a href="#sic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple IRC client.
> Part of the suckless tools.
> More information: <https://tools.suckless.org/sic/>.

#### Connect to the default host (irc.ofct.net) with the nickname set in the `$USER` environment variable:
```shell
sic
```
#### Connect to a given host, using a given nickname:
```shell
sic -h {{host}} -n {{nickname}}
```
#### Connect to a given host, using a given nickname and password:
```shell
sic -h {{host}} -n {{nickname}} -k {{password}}
```
#### Join a channel:
```shell
:j #{{channel}}<Enter>
```
#### Send a message to a channel or user:
```shell
:m #{{channel|user}}<Enter>
```
#### Set default channel or user:
```shell
:s #{{channel|user}}<Enter>
```
{% endraw %}