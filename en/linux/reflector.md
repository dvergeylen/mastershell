---
layout: default
title: "reflector"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reflector">
  <a href="/en/linux/reflector.html">reflector</a> <a href="#reflector"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch script to fetch and sort mirrorlists.

#### Get all mirrors, sort for download speed and save them:
```shell
sudo reflector --sort {{rate}} --save {{/etc/pacman.d/mirrorlist}}
```
#### Only get German HTTPS mirrors:
```shell
reflector --country {{Germany}} --protocol {{https}}
```
#### Only get the 10 recently sync'd mirrors:
```shell
reflector --latest {{10}}
```
{% endraw %}