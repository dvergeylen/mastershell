---
layout: default
title: "gpg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpg">
  <a href="/de/common/gpg.html">gpg</a> <a href="#gpg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard.
> Weitere Informationen: <https://gnupg.org>.

#### Signiere `doc.txt` ohne Verschlüsselung (Ausabe nach `doc.txt.asc`):
```shell
gpg --clearsign {{doc.txt}}
```
#### Verschlüssle `doc.txt` für alice@beispiel.de (Ausgabe nach `doc.txt.gpg`):
```shell
gpg --encrypt --recipient {{alice@beispiel.de}} {{doc.txt}}
```
#### Verschlüssle `doc.txt` nur mit Passwort (Ausgabe nach `doc.txt.gpg`):
```shell
gpg --symmetric {{doc.txt}}
```
#### Entschlüssle `doc.txt.gpg` (Ausgabe nach stdout):
```shell
gpg --decrypt {{doc.txt.gpg}}
```
#### Importiere einen Öffentlichen Schlüssel:
```shell
gpg --import {{schlüssel.gpg}}
```
#### Exportiere den öffentlichen Schlüssel von alice@beispiel.de (Ausgabe nach stdout):
```shell
gpg --export --armor {{alice@beispiel.de}}
```
#### Exportiere den privaten Schlüssel von alice@beispiel.de (Ausgabe nach stdout):
```shell
gpg --export-secret-keys --armor {{alice@beispiel.de}}
```
{% endraw %}