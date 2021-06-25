---
layout: default
title: "nix-collect-garbage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nix-collect-garbage">
  <a href="/en/common/nix-collect-garbage.html">nix-collect-garbage</a> <a href="#nix-collect-garbage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete unused and unreachable nix store paths.
> Generations can be listed using `nix-env --list-generations`.
> More information: <https://nixos.org/releases/nix/latest/manual/#sec-nix-collect-garbage>.

#### Delete all store paths unused by current generations of each profile:
```shell
sudo nix-collect-garbage --delete-old
```
#### Simulate the deletion of old store paths:
```shell
sudo nix-collect-garbage --delete-old --dry-run
```
#### Delete all store paths older than 30 days:
```shell
sudo nix-collect-garbage --delete-older-than {{30d}}
```
{% endraw %}