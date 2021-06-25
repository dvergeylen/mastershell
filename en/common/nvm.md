---
layout: default
title: "nvm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nvm">
  <a href="/en/common/nvm.html">nvm</a> <a href="#nvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install, uninstall or switch between Node.js versions.
> Supports version numbers like "0.12" or "v4.2", and labels like "stable", "system", etc.
> More information: <https://github.com/creationix/nvm>.

#### Install a specific version of Node.js:
```shell
nvm install {{node_version}}
```
#### Use a specific version of Node.js in the current shell:
```shell
nvm use {{node_version}}
```
#### Set the default Node.js version:
```shell
nvm alias default {{node_version}}
```
#### List all available Node.js versions and highlight the default one:
```shell
nvm list
```
#### Uninstall a given Node.js version:
```shell
nvm uninstall {{node_version}}
```
#### Launch the REPL of a specific version of Node.js:
```shell
nvm run {{node_version}} --version
```
#### Execute a script in a specific version of Node.js:
```shell
nvm exec {{node_version}} node {{app.js}}
```
{% endraw %}