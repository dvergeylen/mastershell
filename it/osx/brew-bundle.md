---
layout: default
title: "brew bundle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew-bundle">
  <a href="/it/osx/brew-bundle.html">brew bundle</a> <a href="#brew-bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bundler per Homebrew, Homebrew Cask e per il Mac App Store.
> Maggiori informazioni: <https://github.com/Homebrew/homebrew-bundle>.

#### Installa un pacchetto da un Brewfile nel percorso corrente:
```shell
brew bundle
```
#### Installa pacchetti da un Brewfile specifico in un percorso specifico:
```shell
brew bundle --file={{percorso/del/file}}
```
#### Crea un Brewfile con tutti i pacchetti installati:
```shell
brew bundle dump
```
#### Disinstalla tutti i pacchetti non specificati nel Brewfile:
```shell
brew bundle cleanup --force
```
#### Controlla se c'è qualcosa da installare o da aggiornare nel Brewfile:
```shell
brew bundle check
```
#### Mostra una lista di tutte le righe presenti nel Brewfile:
```shell
brew bundle list --all
```
{% endraw %}