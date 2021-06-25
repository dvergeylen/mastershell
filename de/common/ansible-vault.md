---
layout: default
title: "ansible-vault"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-vault">
  <a href="/de/common/ansible-vault.html">ansible-vault</a> <a href="#ansible-vault"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verschlüsselt und entschlüsselt Werte, Datenstrukturen und Dateien innerhalb von Ansible-Projekten.
> Weitere Informationen: <https://docs.ansible.com/ansible/latest/user_guide/vault.html>.

#### Erstelle eine neue verschlüsselte Vault-Datei mit einer Eingabeaufforderung für ein Passwort:
```shell
ansible-vault create {{vault_datei}}
```
#### Erstelle eine neue verschlüsselte Vault-Datei mit einer Vault-Schlüsseldatei, um sie zu verschlüsseln:
```shell
ansible-vault create --vault-password-file={{schlüsseldatei}} {{vault_datei}}
```
#### Verschlüssle eine vorhandene Datei mit einer optionalen Schlüsseldatei:
```shell
ansible-vault encrypt --vault-password-file={{schlüsseldatei}} {{vault_file}}
```
#### Verschlüssle eine Zeichenfolge mit dem verschlüsselten Zeichenfolgenformat von Ansible, wobei interaktive Eingabeaufforderungen angezeigt werden:
```shell
ansible-vault encrypt_string
```
#### Zeige eine verschlüsselten Datei an, wobei eine Kennwortdatei zum Entschlüsseln verwendet wird:
```shell
ansible-vault view --vault-password-file={{schlüsseldatei}} {{vault_datei}}
```
#### Verschlüssle eine bereits verschlüsselte Vault Datei mit einer neuen Kennwortdatei neu:
```shell
ansible-vault rekey --vault-password-file={{alte_schlüsseldatei}} --new-vault-password-file={{neue_schlüsseldatei}} {{vault_datei}}
```
{% endraw %}