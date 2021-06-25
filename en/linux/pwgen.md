---
layout: default
title: "pwgen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pwgen">
  <a href="/en/linux/pwgen.html">pwgen</a> <a href="#pwgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate pronounceable passwords.

#### Generate random password with s[y]mbols:
```shell
pwgen -y {{length}}
```
#### Generate secure, hard-to-memorize passwords:
```shell
pwgen -s {{length}}
```
#### Generate password with at least one capital letter in them:
```shell
pwgen -c {{length}}
```
{% endraw %}