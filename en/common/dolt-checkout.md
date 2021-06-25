---
layout: default
title: "dolt checkout"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dolt-checkout">
  <a href="/en/common/dolt-checkout.html">dolt checkout</a> <a href="#dolt-checkout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Checkout the work tree or tables to a specific branch or commit.
> More information: <https://github.com/dolthub/dolt>.

#### Switch to a branch:
```shell
dolt checkout {{branch_name}}
```
#### Revert unstaged changes to a table:
```shell
dolt checkout {{table}}
```
#### Create new branch and switch to it:
```shell
dolt checkout -b {{branch_name}}
```
#### Create new branch based on a specified commit and switch to it:
```shell
dolt checkout -b {{branch_name}} {{commit}}
```
{% endraw %}