---
layout: default
title: "packtpub"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="packtpub">
  <a href="/en/common/packtpub.html">packtpub</a> <a href="#packtpub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Download freely offered books from packtpub.com.
> More information: <https://github.com/vladimyr/packtpub-cli>.

#### Download the daily offer book into the current directory with the specified book format (defaults to `pdf`):
```shell
packtpub download --type {{pdf|ebup|mobi}}
```
#### Download the daily offer book into the specified directory:
```shell
packtpub download --dir {{path/to/directory}}
```
#### Start an interactive login to packtpub.com:
```shell
packtpub login
```
#### Log out from packtpub.com:
```shell
packtpub logout
```
#### Display the daily offer:
```shell
packtpub view-offer
```
#### Open the daily offer in the default web browser:
```shell
packtpub view-offer
```
#### Display the currently logged-in user:
```shell
packtpub whoami
```
{% endraw %}