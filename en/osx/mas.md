---
layout: default
title: "mas"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mas">
  <a href="/en/osx/mas.html">mas</a> <a href="#mas"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface for the Mac App Store.
> More information: <https://github.com/mas-cli/mas>.

#### Sign into the Mac App Store for the first time:
```shell
mas signin {{user@example.com}}
```
#### Show all installed applications and their product identifiers:
```shell
mas list
```
#### Search for an application, displaying the price alongside the results:
```shell
mas search {{application}} --price
```
#### Install or update an application:
```shell
mas install {{product_identifier}}
```
#### Install all pending updates:
```shell
mas upgrade
```
{% endraw %}