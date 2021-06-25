---
layout: default
title: "brew cask"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew-cask">
  <a href="/en/osx/brew-cask.html">brew cask</a> <a href="#brew-cask"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package manager for macOS applications distributed as binaries.
> More information: <https://github.com/Homebrew/homebrew-cask>.

#### Search for formulas and casks:
```shell
brew search {{text}}
```
#### Install a cask:
```shell
brew cask install {{cask_name}}
```
#### List all installed casks:
```shell
brew list --cask
```
#### List installed casks that have newer versions available:
```shell
brew outdated --cask
```
#### Upgrade an installed cask (if no cask name is given, all installed casks are upgraded):
```shell
brew upgrade --cask {{cask_name}}
```
#### Uninstall a cask:
```shell
brew cask uninstall {{cask_name}}
```
#### Uninstall a cask and remove related settings and files:
```shell
brew cask zap {{cask_name}}
```
#### Display information about a given cask:
```shell
brew cask info {{cask_name}}
```
{% endraw %}