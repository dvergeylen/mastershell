---
layout: default
title: "pacman --sync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman---sync">
  <a href="/en/linux/pacman-sync.html">pacman --sync</a> <a href="#pacman---sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Install a new package:
```shell
sudo pacman --sync {{package_name}}
```
#### Synchronize and update all packages (add `--downloadonly` to download the packages and not update them):
```shell
sudo pacman --sync --refresh --sysupgrade
```
#### Update all packages and install a new one without prompting:
```shell
sudo pacman --sync --refresh --sysupgrade --noconfirm {{package_name}}
```
#### Search the package database for a regular expression or keyword:
```shell
pacman --sync --search "{{search_pattern}}"
```
#### Display information about a package:
```shell
pacman --sync --info {{package_name}}
```
#### Overwrite conflicting files during a package update:
```shell
sudo pacman --sync --refresh --sysupgrade --overwrite {{path/to/file}}
```
#### Synchronize and update all packages, but ignore a specific package (can be used more than once):
```shell
sudo pacman --sync --refresh --sysupgrade --ignore {{package_name}}
```
#### Remove not installed packages and unused repositories from the cache (use two `--clean` flags to clean all packages):
```shell
sudo pacman --sync --clean
```
{% endraw %}