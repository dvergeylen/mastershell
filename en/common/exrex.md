---
layout: default
title: "exrex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exrex">
  <a href="/en/common/exrex.html">exrex</a> <a href="#exrex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate all/random matching strings for a regular expression.
> It can also simplify regular expressions.
> More information: <https://github.com/asciimoo/exrex>.

#### Generate all possible strings that match a regular expression:
```shell
exrex '{{regular_expression}}'
```
#### Generate a random string that matches a regular expression:
```shell
exrex --random '{{regular_expression}}'
```
#### Generate at most 100 strings that match a regular expression:
```shell
exrex --max-number {{100}} '{{regular_expression}}'
```
#### Generate all possible strings that match a regular expression, joined together by a custom delimiter string:
```shell
exrex --delimiter "{{, }}" '{{regular_expression}}'
```
#### Print count of all possible strings that match a regular expression:
```shell
exrex --count '{{regular_expression}}'
```
#### Simplify a regular expression:
```shell
exrex --simplify '{{ab|ac}}'
```
#### Print eyes:
```shell
exrex '{{[oO0](_)[oO0]}}'
```
#### Print a boat:
```shell
exrex '{{( {20}(\| *\\|-{22}|\|)|\.={50}| ( ){0,5}\\\.| {12}~{39})}}'
```
{% endraw %}