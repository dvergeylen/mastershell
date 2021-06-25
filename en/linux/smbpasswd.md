---
layout: default
title: "smbpasswd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="smbpasswd">
  <a href="/en/linux/smbpasswd.html">smbpasswd</a> <a href="#smbpasswd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change a user's SMB password.
> Samba users must also have a local Unix account.

#### Change the current user's SMB password:
```shell
smbpasswd
```
#### Add a specified user to Samba and set password(user should already exist in system):
```shell
smbpasswd -a {{username}}
```
#### Modify an existing Samba user's password:
```shell
smbpasswd {{username}}
```
#### Delete a Samba user:
```shell
smbpasswd -x {{username}}
```
{% endraw %}