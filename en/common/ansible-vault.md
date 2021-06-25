---
layout: default
title: "ansible-vault"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-vault">
  <a href="/en/common/ansible-vault.html">ansible-vault</a> <a href="#ansible-vault"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encrypts & decrypts values, data structures and files within Ansible projects.
> More information: <https://docs.ansible.com/ansible/latest/user_guide/vault.html#id17>.

#### Create a new encrypted vault file with a prompt for a password:
```shell
ansible-vault create {{vault_file}}
```
#### Create a new encrypted vault file using a vault key file to encrypt it:
```shell
ansible-vault create --vault-password-file={{password_file}} {{vault_file}}
```
#### Encrypt an existing file using an optional password file:
```shell
ansible-vault encrypt --vault-password-file={{password_file}} {{vault_file}}
```
#### Encrypt a string using Ansible's encrypted string format, displaying interactive prompts:
```shell
ansible-vault encrypt_string
```
#### View an encrypted file, using a password file to decrypt:
```shell
ansible-vault view --vault-password-file={{password_file}} {{vault_file}}
```
#### Re-key already encrypted vault file with a new password file:
```shell
ansible-vault rekey --vault-password-file={{old_password_file}} --new-vault-password-file={{new_password_file}} {{vault_file}}
```
{% endraw %}