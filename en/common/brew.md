---
layout: default
title: "brew"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew">
  <a href="/en/common/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package manager for macOS and Linux.
> More information: <https://brew.sh>.

#### Install the latest stable version of a formula or cask (use `--devel` for development versions):
```shell
brew install {{formula}}
```
#### List all installed formulae and casks:
```shell
brew list
```
#### Upgrade an installed formula or cask (if none is given, all installed formulae/casks are upgraded):
```shell
brew upgrade {{formula}}
```
#### Fetch the newest version of Homebrew and of all formulae and casks from the Homebrew source repository:
```shell
brew update
```
#### Show formulae and casks that have a more recent version available:
```shell
brew outdated
```
#### Search for available formulae (i.e. packages) and casks (i.e. native packages):
```shell
brew search {{text}}
```
#### Display information about a formula or a cask (version, installation path, dependencies, etc.):
```shell
brew info {{formula}}
```
#### Check the local Homebrew installation for potential problems:
```shell
brew doctor
```
{% endraw %}