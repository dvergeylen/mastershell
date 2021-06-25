---
layout: default
title: "gpg2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpg2">
  <a href="/de/common/gpg2.html">gpg2</a> <a href="#gpg2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard 2.
> Siehe `gpg` für GNU Privacy Guard 1.
> Weitere Informationen: <https://docs.releng.linuxfoundation.org/en/latest/gpg.html>.

#### Liste alle importierten Schlüssel auf:
```shell
gpg2 --list-keys
```
#### Verschlüssle eine bestimme Datei für einen bestimmten Empfänger und schreibe den Output in eine neue `.gpg` Datei:
```shell
gpg2 --encrypt --recipient {{hans@beispiel.de}} {{pfad/zu/datei.txt}}
```
#### Verschlüssle eine bestimmte Datei nur mit einem Passwort und schreibe den Output in eine neue `.gpg` Datei:
```shell
gpg2 --symmetric {{pfad/zu/datei.txt}}
```
#### Verschlüssle eine bestimmte Datei und schreibe des Ergebnis auf STDOUT:
```shell
gpg2 --decrypt {{pfad/zu/datei.txt.gpg}}
```
#### Importiere einen öffentlichen Schlüssel:
```shell
gpg2 --import {{pfad/zu/öffentlichem_schlüssel.gpg}}
```
#### Exportiere den öffentlichen Schlüssel einer bestimmten Email-Adresse nach STDOUT:
```shell
gpg2 --export --armor {{hans@beispiel.de}}
```
#### Exportiere den privaten Schlüssel einer bestimmten Email-Adresse nach STDOUT:
```shell
gpg2 --export-secret-keys --armor {{hans@beispiel.de}}
```
{% endraw %}