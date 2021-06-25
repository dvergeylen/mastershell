---
layout: default
title: "sshpass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sshpass">
  <a href="/en/common/sshpass.html">sshpass</a> <a href="#sshpass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An ssh password provider.
> It works by creating a TTY, feeding the password into it, and then redirecting stdin to the ssh session.

#### Connect to a remote server using a password supplied on a file descriptor (in this case, stdin):
```shell
sshpass -d {{0}} ssh {{user}}@{{hostname}}
```
#### Connect to a remote server with the password supplied as an option, and automatically accept unknown ssh keys:
```shell
sshpass -p {{password}} ssh -o StrictHostKeyChecking=no {{user}}@{{hostname}}
```
#### Connect to a remote server using the first line of a file as the password, automatically accept unknown ssh keys, and launch a command:
```shell
sshpass -f {{file}} ssh -o StrictHostKeyChecking=no {{user}}@{{hostname}} "{{command}}"
```
{% endraw %}