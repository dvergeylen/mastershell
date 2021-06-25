---
layout: default
title: "authconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="authconfig">
  <a href="/en/linux/authconfig.html">authconfig</a> <a href="#authconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI interface for configuring system authentication resources.

#### Display the current configuration (or dry run):
```shell
authconfig --test
```
#### Configure the server to use a different password hashing algorithm:
```shell
authconfig --update --passalgo={{algorithm}}
```
#### Enable LDAP authentication:
```shell
authconfig --update --enableldapauth
```
#### Disable LDAP authentication:
```shell
authconfig --update --disableldapauth
```
#### Enable Network Information Service (NIS):
```shell
authconfig --update --enablenis
```
#### Enable Kerberos:
```shell
authconfig --update --enablekrb5
```
#### Enable Winbind (Active Directory) authentication:
```shell
authconfig --update --enablewinbindauth
```
#### Enable local authorization:
```shell
authconfig --update --enablelocauthorize
```
{% endraw %}