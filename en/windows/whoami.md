---
layout: default
title: "whoami"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whoami">
  <a href="/en/windows/whoami.html">whoami</a> <a href="#whoami"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display details about the current user.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/whoami>.

#### Display the username of the current user:
```shell
whoami
```
#### Display the groups that the current user is a member of:
```shell
whoami /groups
```
#### Display the privileges of the current user:
```shell
whoami /priv
```
#### Display the user principal name (UPN) of the current user:
```shell
whoami /upn
```
#### Display the logon id of the current user:
```shell
whoami /logonid
```
{% endraw %}