---
layout: default
title: "fdesetup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fdesetup">
  <a href="/en/osx/fdesetup.html">fdesetup</a> <a href="#fdesetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set and retrieve FileVault related information.

#### List current FileVault enabled users:
```shell
sudo fdesetup list
```
#### Get current FileVault status:
```shell
fdesetup status
```
#### Add FileVault enabled user:
```shell
sudo fdesetup add -usertoadd user1
```
#### Enable FileVault:
```shell
sudo fdesetup enable
```
#### Disable FileVault:
```shell
sudo fdesetup disable
```
{% endraw %}