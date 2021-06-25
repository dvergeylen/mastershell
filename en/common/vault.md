---
layout: default
title: "vault"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vault">
  <a href="/en/common/vault.html">vault</a> <a href="#vault"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI to interact with HashiCorp Vault.
> More information: <https://www.vaultproject.io/docs/commands>.

#### Connect to a Vault server and initialize a new encrypted data store:
```shell
vault init
```
#### Unseal (unlock) the vault, by providing one of the key shares needed to access the encrypted data store:
```shell
vault unseal {{key-share-x}}
```
#### Authenticate the CLI client against the Vault server, using an authentication token:
```shell
vault auth {{authentication_token}}
```
#### Store a new secret in the vault, using the generic back-end called "secret":
```shell
vault write secret/{{hello}} value={{world}}
```
#### Read a value from the vault, using the generic back-end called "secret":
```shell
vault read secret/{{hello}}
```
#### Read a specific field from the value:
```shell
vault read -field={{field_name}} secret/{{hello}}
```
#### Seal (lock) the Vault server, by removing the encryption key of the data store from memory:
```shell
vault seal
```
{% endraw %}