---
layout: default
title: "nodenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nodenv">
  <a href="/en/common/nodenv.html">nodenv</a> <a href="#nodenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to manage Node.js versions.
> More information: <https://github.com/nodenv/nodenv>.

#### Install a specific version of Node.js:
```shell
nodenv install {{version}}
```
#### Display a list of available versions:
```shell
nodenv install --list
```
#### Use a specific version of Node.js across the whole system:
```shell
nodenv global {{version}}
```
#### Use a specific version of Node.js with a directory:
```shell
nodenv local {{version}}
```
#### Display the Node.js version for the current directory:
```shell
nodenv version
```
#### Display the location of a Node.js installed command (e.g. `npm`):
```shell
nodenv which {{command}}
```
{% endraw %}