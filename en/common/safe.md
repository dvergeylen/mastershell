---
layout: default
title: "safe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="safe">
  <a href="/en/common/safe.html">safe</a> <a href="#safe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI to interact with HashiCorp Vault.
> More information: <https://github.com/starkandwayne/safe>.

#### Add a safe target:
```shell
safe target {{vault_addr}} {{target_name}}
```
#### Authenticate the CLI client against the Vault server, using an authentication token:
```shell
safe auth {{authentication_token}}
```
#### Print the environment variables describing the current target:
```shell
safe env
```
#### Display a tree hierarchy of all reachable keys for a given path:
```shell
safe tree {{path}}
```
#### Move a secret from one path to another:
```shell
safe move {{old/path/to/secret}} {{new/path/to/secret}}
```
#### Generate a new 2048-bit SSH key-pair and store it:
```shell
safe ssh {{2048}} {{path/to/secret}}
```
#### Set non-sensitive keys for a secret:
```shell
safe set {{path/to/secret}} {{key}}={{value}}
```
#### Set auto-generated password in a secret:
```shell
safe gen {{path/to/secret}} {{key}}
```
{% endraw %}