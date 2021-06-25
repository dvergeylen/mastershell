---
layout: default
title: "opam"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="opam">
  <a href="/en/common/opam.html">opam</a> <a href="#opam"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OCaml Package Manager.
> Manage OCaml compilers, tools and libraries.
> More information: <https://opam.ocaml.org/>.

#### Initialize opam for first use:
```shell
opam init
```
#### Search for packages:
```shell
opam search {{package_name}}
```
#### Install a package and all of its dependencies:
```shell
opam install {{package_name}}
```
#### Display detailed information about a package:
```shell
opam show {{package_name}}
```
#### List all installed packages:
```shell
opam list
```
#### Update the local package database:
```shell
opam update
```
#### Upgrade all installed packages:
```shell
opam upgrade
```
#### Display all commands:
```shell
opam help
```
{% endraw %}