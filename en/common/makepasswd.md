---
layout: default
title: "makepasswd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="makepasswd">
  <a href="/en/common/makepasswd.html">makepasswd</a> <a href="#makepasswd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate and encrypt passwords.
> More information: <https://manpages.debian.org/stretch/makepasswd/makepasswd.1.en.html>.

#### Generate a random password (8 to 10 characters long, containing letters and numbers):
```shell
makepasswd
```
#### Generate a 10 characters long password:
```shell
makepasswd --chars {{10}}
```
#### Generate a 5 to 10 characters long password:
```shell
makepasswd --minchars {{5}} --maxchars {{10}}
```
#### Generate a password containing only the characters "b", "a" or "r":
```shell
makepasswd --string {{bar}}
```
{% endraw %}