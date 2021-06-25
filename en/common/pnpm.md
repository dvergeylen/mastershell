---
layout: default
title: "pnpm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pnpm">
  <a href="/en/common/pnpm.html">pnpm</a> <a href="#pnpm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fast, disk space efficient package manager for Node.js.
> Manage Node.js projects and their module dependencies.
> More information: <https://pnpm.io>.

#### Interactively create a `package.json` file:
```shell
pnpm init
```
#### Download all the packages listed as dependencies in `package.json`:
```shell
pnpm install
```
#### Download a specific version of a package and add it to the list of dependencies in `package.json`:
```shell
pnpm install {{module_name}}@{{version}}
```
#### Download a package and add it to the list of dev dependencies in `package.json`:
```shell
pnpm install --dev {{module_name}}
```
#### Download a package and install it globally:
```shell
pnpm install -g {{module_name}}
```
#### Uninstall a package and remove it from the list of dependencies in `package.json`:
```shell
pnpm uninstall {{module_name}}
```
#### Print a tree of locally installed modules:
```shell
pnpm list
```
#### List top-level [g]lobally installed modules:
```shell
pnpm list -g --depth={{0}}
```
{% endraw %}