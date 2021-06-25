---
layout: default
title: "brew cask"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew-cask">
  <a href="/it/osx/brew-cask.html">brew cask</a> <a href="#brew-cask"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di pacchetti per applicazioni macOS distribuite sotto forma di file binari.
> Maggiori informazioni: <https://github.com/Homebrew/homebrew-cask>.

#### Cerca formule e cask:
```shell
brew search {{testo}}
```
#### Installa un cask:
```shell
brew cask install {{nome_del_cask}}
```
#### Elenca tutti i cask installati:
```shell
brew cask list
```
#### Elenca i cask installati con versioni più nuove disponibili:
```shell
brew cask outdated
```
#### Aggiorna un cask installato (se non viene fornito il nome di nessun cask, tutti i cask saranno aggiornati):
```shell
brew cask upgrade {{nome_del_cask}}
```
#### Disinstalla un cask:
```shell
brew cask uninstall {{nome_del_cask}}
```
#### Disinstalla un cask e rimuovi i relativi file e impostazioni:
```shell
brew cask zap {{nome_del_cask}}
```
#### Mostra informazioni su uno specifico cask:
```shell
brew cask info {{nome_del_cask}}
```
{% endraw %}