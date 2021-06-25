---
layout: default
title: "compgen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="compgen">
  <a href="/en/osx/compgen.html">compgen</a> <a href="#compgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A built-in command for auto-completion in bash, which is called on pressing TAB key twice.

#### List all commands that you could run:
```shell
compgen -c
```
#### List all aliases:
```shell
compgen -a
```
#### List all functions that you could run:
```shell
compgen -A function
```
#### Show shell reserved key words:
```shell
compgen -k
```
#### See all available commands/aliases starting with 'ls':
```shell
compgen -ac {{ls}}
```
{% endraw %}