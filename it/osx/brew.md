---
layout: default
title: "brew"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew">
  <a href="/it/osx/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di pacchetti per macOS.
> Maggiori informazioni: <https://brew.sh>.

#### Cerca formule e cask:
```shell
brew search {{testo}}
```
#### Installa l'ultima versione stabile di una formula (usa `--devel` per le versioni in sviluppo):
```shell
brew install {{formula}}
```
#### Mostra tutte le formule installate:
```shell
brew list
```
#### Mostra le formule installate che non sono dipendenze di un'altra formula installata:
```shell
brew leaves
```
#### Aggiorna una formula installata (se non viene fornito il nome di nessuna formula, tutte le formule installate verranno aggiornate):
```shell
brew upgrade {{formula}}
```
#### Trova la versione più aggiornata di Homebrew e di tutte le formule da GitHub:
```shell
brew update
```
#### Mostra le informazioni su una specifica formula (versione, percorso di installazione, dipendenze, ecc...):
```shell
brew info {{formula}}
```
#### Verifica se la versione installata di Homebrew presenta dei problemi:
```shell
brew doctor
```
{% endraw %}