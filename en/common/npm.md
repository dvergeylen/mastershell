---
layout: default
title: "npm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="npm">
  <a href="/en/common/npm.html">npm</a> <a href="#npm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> JavaScript and Node.js package manager.
> Manage Node.js projects and their module dependencies.
> More information: <https://www.npmjs.com/>.

#### Interactively create a `package.json` file:
```shell
npm init
```
#### Download all the packages listed as dependencies in package.json:
```shell
npm install
```
#### Download a specific version of a package and add it to the list of dependencies in `package.json`:
```shell
npm install {{module_name}}@{{version}}
```
#### Download a package and add it to the list of dev dependencies in `package.json`:
```shell
npm install {{module_name}} --save-dev
```
#### Download a package and install it globally:
```shell
npm install --global {{module_name}}
```
#### Uninstall a package and remove it from the list of dependencies in `package.json`:
```shell
npm uninstall {{module_name}}
```
#### Print a tree of locally-installed dependencies:
```shell
npm list
```
#### List top-level globally installed modules:
```shell
npm list --global --depth={{0}}
```
{% endraw %}