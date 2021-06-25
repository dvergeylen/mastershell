---
layout: default
title: "pass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pass">
  <a href="/en/common/pass.html">pass</a> <a href="#pass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for storing and reading passwords or other sensitive data.
> All data is GPG-encrypted, and managed with a Git repository.
> More information: <https://www.passwordstore.org>.

#### Initialize (or re-encrypt) the storage using one or more GPG IDs:
```shell
pass init {{gpg_id_1}} {{gpg_id_2}}
```
#### Save a new password and additional information (press Ctrl + D on a new line to complete):
```shell
pass insert --multiline {{path/to/data}}
```
#### Edit an entry:
```shell
pass edit {{path/to/data}}
```
#### Copy a password (first line of the data file) to the clipboard:
```shell
pass -c {{path/to/data}}
```
#### List the whole store tree:
```shell
pass
```
#### Generate a new random password with a given length, and copy it to the clipboard:
```shell
pass generate -c {{path/to/data}} {{num}}
```
#### Initialize a new Git repository (any changes done by pass will be committed automatically):
```shell
pass git init
```
{% endraw %}