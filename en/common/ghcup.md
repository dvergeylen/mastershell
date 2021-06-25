---
layout: default
title: "ghcup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ghcup">
  <a href="/en/common/ghcup.html">ghcup</a> <a href="#ghcup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Haskell toolchain installer.
> Install, manage, and update Haskell toolchains.
> More information: <https://gitlab.haskell.org/haskell/ghcup-hs>.

#### Start the interactive TUI:
```shell
ghcup tui
```
#### List available GHC/cabal versions:
```shell
ghcup list
```
#### Install the recommended GHC version:
```shell
ghcup install ghc
```
#### Install a specific GHC version:
```shell
ghcup install ghc {{version}}
```
#### Set the currently "active" GHC version:
```shell
ghcup set ghc {{version}}
```
#### Install cabal-install:
```shell
ghcup install cabal
```
#### Update `ghcup` itself:
```shell
ghcup upgrade
```
{% endraw %}