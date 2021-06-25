---
layout: default
title: "age"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="age">
  <a href="/de/common/age.html">age</a> <a href="#age"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein einfaches, modernes und sicheres Dateiverschlüsselungswerkzeug.
> Weitere Informationen: <https://age-encryption.org>.

#### Generiere eine verschlüsselte Datei, die mit einer Passphrase entschlüsselt werden kann:
```shell
age --passphrase --output {{pfad/zu/verschlüsselter_datei}} {{pfad/zu/unverschlüsselter_datei}}
```
#### Generiere ein Schlüsselpaar, speichere dabei den privaten Schlüssel in einer unverschlüsselten Datei und gib den öffentlichen Schlüssel zu stdout aus:
```shell
age-keygen --output {{pfad/zu/datei}}
```
#### Verschlüssle eine Datei mit einem oder mehr öffentlichen Schlüsseln, die als Zeichenketten eingegeben werden:
```shell
age --recipient {{öffentlicher_schlüssel_1}} --recipient {{öffentlicher_schlüssel_2}} {{pfad/zu/unverschlüsselter_datei}} --output {{pfad/zu/verschlüsselter_datei}}
```
#### Verschlüssle eine Datei mit einem oder mehr öffentlichen Schlüsseln, die in einer Empfängerdatei angegeben sind:
```shell
age --recipients-file {{pfad/zu/empfängerdatei}} {{pfad/zu/unverschlüsselter_datei}} --output {{pfad/zu/verschlüsselter_datei}}
```
#### Entschlüssle eine Datei mit einer Passphrase:
```shell
age --decrypt --output {{pfad/zu/entschlüsselter_datei}} {{pfad/zu/verschlüsselter_datei}}
```
#### Entschlüssle eine Datei mit einer privaten Schlüsseldatei:
```shell
age --decrypt --identity {{pfad/zu/privater_schlüsseldatei}} --output {{pfad/zu/entschlüsselter_datei}} {{pfad/zu/verschlüsselter_datei}}
```
{% endraw %}