---
layout: default
title: "brew bundle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew-bundle">
  <a href="/de/osx/brew-bundle.html">brew bundle</a> <a href="#brew-bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bundler für Homebrew, Homebrew Cask und den Mac App Store.
> Weitere Informationen: <https://github.com/Homebrew/homebrew-bundle>.

#### Installiere Pakete aus einer Brewfile im aktuellen Pfad:
```shell
brew bundle
```
#### Installiere Pakete aus einer bestimmten Brewfile:
```shell
brew bundle --file={{pfad/zu/brewfile}}
```
#### Gib eine Liste mit allen installierten Paketen aus:
```shell
brew bundle dump
```
#### Deinstalliere Pakete, die nicht in der Brewfile aufgelisted sind:
```shell
brew bundle cleanup --force
```
#### Prüfe, ob von einem Paket die aktuellste Version installiert ist:
```shell
brew bundle check
```
#### Zeige alle Pakete, die in der Brewfile aufgelistet sind:
```shell
brew bundle list --all
```
{% endraw %}