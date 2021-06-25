---
layout: default
title: "lpass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lpass">
  <a href="/en/common/lpass.html">lpass</a> <a href="#lpass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface for the LastPass password manager.
> More information: <https://github.com/lastpass/lastpass-cli>.

#### Log in to your LastPass account, by entering your master password when prompted:
```shell
lpass login {{username}}
```
#### Show login status:
```shell
lpass status
```
#### List all sites grouped by category:
```shell
lpass ls
```
#### Generate a new password for gmail.com with the identifier `myinbox` and add to LastPass:
```shell
lpass generate --username {{username}} --url {{gmail.com}} {{myinbox}} {{password_length}}
```
#### Show password for a specified entry:
```shell
lpass show {{myinbox}} --password
```
{% endraw %}