---
layout: default
title: "Medusa"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="medusa">
  <a href="/en/linux/medusa.html">Medusa</a> <a href="#medusa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A modular and parallel login brute-forcer for a variety of protocols.

#### Execute brute force against an FTP server using a file containing usernames and a file containing passwords:
```shell
medusa -M ftp -h host -U {{path/to/username_file}} -P {{path/to/password_file}}
```
#### Execute a login attempt against a HTTP server using the username, password and user-agent specified:
```shell
medusa -M HTTP -h host -u {{username}} -p {{password}} -m USER-AGENT:"{{Agent}}"
```
#### Execute a brute force against a MySQL server using a file containing usernames and a hash:
```shell
medusa -M mysql -h host -U {{path/to/username_file}} -p {{hash}} -m PASS:HASH
```
#### Execute a brute force against a list of SMB servers using a username and a pwdump file:
```shell
medusa -M smbnt -H {{path/to/hosts_file}} -C {{path/to/pwdump_file}} -u {{username}} -m PASS:HASH
```
{% endraw %}