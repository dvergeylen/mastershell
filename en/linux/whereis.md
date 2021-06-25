---
layout: default
title: "whereis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whereis">
  <a href="/en/linux/whereis.html">whereis</a> <a href="#whereis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Locate the binary, source, and manual page files for a command.

#### Locate binary, source and man pages for ssh:
```shell
whereis {{ssh}}
```
#### Locate binary and man pages for ls:
```shell
whereis -bm {{ls}}
```
#### Locate source of gcc and man pages for Git:
```shell
whereis -s {{gcc}} -m {{git}}
```
#### Locate binaries for gcc in `/usr/bin/` only:
```shell
whereis -b -B {{/usr/bin/}} -f {{gcc}}
```
#### Locate unusual binaries (those that have more or less than one binary on the system):
```shell
whereis -u *
```
#### Locate binaries that have unusual manual entries (binaries that have more or less than one manual installed):
```shell
whereis -u -m *
```
{% endraw %}