---
layout: default
title: "htpasswd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="htpasswd">
  <a href="/en/common/htpasswd.html">htpasswd</a> <a href="#htpasswd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manage htpasswd files to protect web server directories using basic authentication.
> More information: <https://httpd.apache.org/docs/current/programs/htpasswd.html>.

#### Create/overwrite htpasswd file:
```shell
htpasswd -c {{path/to/file}} {{username}}
```
#### Add user to htpasswd file or update existing user:
```shell
htpasswd {{path/to/file}} {{username}}
```
#### Add user to htpasswd file in batch mode without an interactive password prompt (for script usage):
```shell
htpasswd -b {{path/to/file}} {{username}} {{password}}
```
#### Delete user from htpasswd file:
```shell
htpasswd -D {{path/to/file}} {{username}}
```
#### Verify user password:
```shell
htpasswd -v {{path/to/file}} {{username}}
```
#### Display a string with username (plain text) and password (md5):
```shell
htpasswd -nbm {{username}} {{password}}
```
{% endraw %}