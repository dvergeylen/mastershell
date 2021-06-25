---
layout: default
title: "pnpx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pnpx">
  <a href="/en/common/pnpx.html">pnpx</a> <a href="#pnpx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Directly execute binaries from npm packages, using `pnpm` instead of `npm`.
> More information: <https://pnpm.io/pnpx-cli>.

#### Execute the binary from a given npm module:
```shell
pnpx {{module_name}}
```
#### Execute a specific binary from a given npm module, in case the module has multiple binaries:
```shell
pnpx --package {{package_name}} {{module_name}}
```
#### Display help:
```shell
pnpx --help
```
{% endraw %}