---
layout: default
title: "hlint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hlint">
  <a href="/en/linux/hlint.html">hlint</a> <a href="#hlint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for suggesting improvements to Haskell code.
> More information: <http://hackage.haskell.org/package/hlint>.

#### Display suggestions for a given file:
```shell
hlint {{path/to/file}} options
```
#### Check all Haskell files and generate a report:
```shell
hlint {{path/to/directory}} --report
```
#### Automatically apply most suggestions:
```shell
hlint {{path/to/file}} --refactor
```
#### Display additional options:
```shell
hlint {{path/to/file}} --refactor-options
```
#### Generate a settings file ignoring all outstanding hints:
```shell
hlint {{path/to/file}} --default > {{.hlint.yaml}}
```
{% endraw %}