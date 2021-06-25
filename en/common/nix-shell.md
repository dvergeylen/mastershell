---
layout: default
title: "nix-shell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nix-shell">
  <a href="/en/common/nix-shell.html">nix-shell</a> <a href="#nix-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Start an interactive shell based on a Nix expression.
> More information: <https://nixos.org/manual/nix/stable/#sec-nix-shell>.

#### Start with nix expression in `shell.nix` or `default.nix` in the current directory:
```shell
nix-shell
```
#### Run shell command in non-interactive shell and exit:
```shell
nix-shell --run "{{command}} {{command_arguments}}"
```
#### Start with expression in `default.nix` in the current directory:
```shell
nix-shell {{default.nix}}
```
#### Start with packages loaded from nixpkgs:
```shell
nix-shell --packages {{package_name_1}} {{package_name_2}}
```
#### Start with packages loaded from specific nixpkgs revision:
```shell
nix-shell --packages {{package_names}} -I nixpkgs={{https://github.com/NixOS/nixpkgs/archive/nixpkgs_revision.tar.gz}}
```
#### Evaluate rest of file in specific interpreter, for use in `#!-scripts` (see <https://nixos.org/manual/nix/stable/#use-as-a-interpreter>):
```shell
nix-shell -i {{interpreter}} --packages {{package_names}}
```
{% endraw %}