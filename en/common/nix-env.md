---
layout: default
title: "nix-env"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nix-env">
  <a href="/en/common/nix-env.html">nix-env</a> <a href="#nix-env"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manipulate or query Nix user environments.
> More information: <https://nixos.org/manual/nix/stable/#sec-nix-env>.

#### List all installed packages:
```shell
nix-env -q
```
#### Query installed packages:
```shell
nix-env -q {{search_term}}
```
#### Query available packages:
```shell
nix-env -qa {{search_term}}
```
#### Install package:
```shell
nix-env -iA nixpkgs.{{pkg_name}}
```
#### Install a package from a URL:
```shell
nix-env -i {{pkg_name}} --file {{example.com}}
```
#### Uninstall package:
```shell
nix-env -e {{pkg_name}}
```
#### Upgrade one package:
```shell
nix-env -u {{pkg_name}}
```
#### Upgrade all packages:
```shell
nix-env -u
```
{% endraw %}