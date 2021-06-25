---
layout: default
title: "dvc checkout"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-checkout">
  <a href="/en/common/dvc-checkout.html">dvc checkout</a> <a href="#dvc-checkout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Checkout data files and directories from cache.
> More information: <https://dvc.org/doc/command-reference/checkout>.

#### Checkout the latest version of all target files and directories:
```shell
dvc checkout
```
#### Checkout to latest version of a specified target:
```shell
dvc checkout {{target}}
```
#### Checkout a specific version of a target from a different Git commit/tag/branch:
```shell
git checkout {{commit_hash|tag|branch}} {{target}} && dvc checkout {{target}}
```
{% endraw %}