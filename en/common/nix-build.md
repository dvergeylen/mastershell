---
layout: default
title: "nix-build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nix-build">
  <a href="/en/common/nix-build.html">nix-build</a> <a href="#nix-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build a Nix expression.
> More information: <https://nixos.org/releases/nix/latest/manual#sec-nix-build>.

#### Build a Nix expression:
```shell
nix-build --attr {{expression_name}}
```
#### Build a sandboxed Nix expression (on non-NixOS):
```shell
nix-build --attr {{expression_name}} --option sandbox true
```
{% endraw %}