---
layout: default
title: "keepass2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="keepass2">
  <a href="/en/common/keepass2.html">keepass2</a> <a href="#keepass2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A light-weight password manager.
> More information: <https://keepass.info>.

#### Start KeePass 2, opening the most recently-opened password database:
```shell
keepass2
```
#### Start KeePass 2, opening a specific password database:
```shell
keepass2 {{path/to/database.kbdx}}
```
#### Use a specific key file to open a password database:
```shell
keepass2 {{path/to/database.kbdx}} -keyfile:{{path/to/key/file.key}}
```
{% endraw %}