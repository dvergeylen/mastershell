---
layout: default
title: "aws-vault"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-vault">
  <a href="/de/common/aws-vault.html">aws-vault</a> <a href="#aws-vault"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Tresor für Entwicklungsumgebungen um AWS Sicherheitsschlüssel sicher speichern und abrufen zu können.
> Weitere Informationen: <https://github.com/99designs/aws-vault>.

#### Füge einen Sicherheitsschlüssel als Profil zu einem Tresor hinzu:
```shell
aws-vault add {{profil}}
```
#### Führe einen Befehl mit AWS Sicherheitsschlüsseln aus dem angegebenen Profil aus:
```shell
aws-vault exec {{profil}} -- {{aws s3 ls}}
```
#### Öffne ein Browserfenster für den Login in die AWS Konsole:
```shell
aws-vault login {{profil}}
```
#### Liste alle Profile zusammen mit deren Sicherheitsschlüsseln und Sitzungen auf:
```shell
aws-vault list
```
#### Rotiere die AWS Sicherheitsschlüssel für ein Profil:
```shell
aws-vault rotate {{profil}}
```
#### Entferne Sicherheitsschlüsseln eines Profils aus dem Tresor:
```shell
aws-vault remove {{profil}}
```
{% endraw %}