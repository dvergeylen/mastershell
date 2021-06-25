---
layout: default
title: "yarn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yarn">
  <a href="/en/common/yarn.html">yarn</a> <a href="#yarn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> JavaScript and Node.js package manager alternative.
> More information: <https://yarnpkg.com>.

#### Install a module globally:
```shell
yarn global add {{module_name}}
```
#### Install all dependencies referenced in the `package.json` file (the `install` is optional):
```shell
yarn install
```
#### Install a module and save it as a dependency to the `package.json` file (add `--dev` to save as a dev dependency):
```shell
yarn add {{module_name}}@{{version}}
```
#### Uninstall a module and remove it from the `package.json` file:
```shell
yarn remove {{module_name}}
```
#### Interactively create a `package.json` file:
```shell
yarn init
```
#### Identify whether a module is a dependency and list other modules that depend upon it:
```shell
yarn why {{module_name}}
```
{% endraw %}