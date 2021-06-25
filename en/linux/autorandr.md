---
layout: default
title: "autorandr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autorandr">
  <a href="/en/linux/autorandr.html">autorandr</a> <a href="#autorandr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Automatically change screen layout.

#### Save the current screen layout:
```shell
autorandr -s {{profile_name}}
```
#### Show the saved profiles:
```shell
autorandr
```
#### Change the profile:
```shell
autorandr -l {{profile_name}}
```
#### Set the default profile:
```shell
autorandr -d {{profile_name}}
```
{% endraw %}