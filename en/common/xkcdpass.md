---
layout: default
title: "xkcdpass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xkcdpass">
  <a href="/en/common/xkcdpass.html">xkcdpass</a> <a href="#xkcdpass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A flexible and scriptable password generator which generates strong passphrases.
> Inspired by XKCD 936.
> More information: <https://github.com/redacted/XKCD-password-generator>.

#### Generate one passphrase with the default options:
```shell
xkcdpass
```
#### Generate one passphrase whose first letters of each word match the provided argument:
```shell
xkcdpass -a {{acrostic}}
```
#### Generate passwords interactively:
```shell
xkcdpass -i
```
{% endraw %}