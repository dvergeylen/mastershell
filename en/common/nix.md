---
layout: default
title: "nix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nix">
  <a href="/en/common/nix.html">nix</a> <a href="#nix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilities for the Nix language and store.
> More information: <https://nixos.org>.

#### Search for a package via its name or description:
```shell
nix search {{search_term}}
```
#### Start a Nix shell with the specified packages available:
```shell
nix run {{nixpkgs.pkg1 nixpkgs.pkg2 nixpkgs.pkg3...}}
```
#### Optimise Nix store disk usage by combining duplicate files:
```shell
nix optimise-store
```
#### Start an interactive environment for evaluating Nix expressions:
```shell
nix repl
```
#### Upgrade Nix to the latest stable version:
```shell
nix upgrade-nix
```
{% endraw %}