---
layout: default
title: "pacman --remove"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---remove">
  <a href="/en/linux/pacman-remove.html">pacman --remove</a> <a href="#pacman---remove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Display help for this subcommand:
```shell
pacman --remove --help
```
#### Remove a package and its dependencies:
```shell
sudo pacman --remove --recursive {{package_name}}
```
#### Remove a package and both its dependencies and configuration files:
```shell
sudo pacman --remove --recursive --nosave {{package_name}}
```
#### Remove a package without prompting:
```shell
sudo pacman --remove --noconfirm {{package_name}}
```
#### Remove orphan packages (installed as dependencies but not required by any package):
```shell
sudo pacman --remove --recursive --nosave $(pacman --query --unrequired --deps --quiet)
```
#### Remove a package and all packages that depend on it:
```shell
sudo pacman --remove --cascade {{package_name}}
```
#### List packages that would be affected (does not remove any packages):
```shell
pacman --remove --print {{package_name}}
```
{% endraw %}