---
layout: default
title: "cabal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cabal">
  <a href="/en/common/cabal.html">cabal</a> <a href="#cabal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface to the Haskell package infrastructure (Cabal).
> Manage Haskell projects and Cabal packages from the Hackage package repository.
> More information: <https://cabal.readthedocs.io/en/latest/intro.html>.

#### Search and list packages from Hackage:
```shell
cabal list {{search_string}}
```
#### Show information about a package:
```shell
cabal info {{package_name}}
```
#### Download and install a package:
```shell
cabal install {{package_name}}
```
#### Create a new Haskell project in the current directory:
```shell
cabal init
```
#### Build the project in the current directory:
```shell
cabal build
```
#### Run tests of the project in the current directory:
```shell
cabal test
```
{% endraw %}