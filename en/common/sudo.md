---
layout: default
title: "sudo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sudo">
  <a href="/en/common/sudo.html">sudo</a> <a href="#sudo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executes a single command as the superuser or another user.
> More information: <https://www.sudo.ws/sudo.html>.

#### Run a command as the superuser:
```shell
sudo {{less /var/log/syslog}}
```
#### Edit a file as the superuser with your default editor:
```shell
sudo --edit {{/etc/fstab}}
```
#### Run a command as another user and/or group:
```shell
sudo --user={{user}} --group={{group}} {{id -a}}
```
#### Repeat the last command prefixed with `sudo` (only in `bash`, `zsh`, etc.):
```shell
sudo !!
```
#### Launch the default shell with superuser privileges and run login-specific files (`.profile`, `.bash_profile`, etc.):
```shell
sudo --login
```
#### Launch the default shell with superuser privileges without changing the environment:
```shell
sudo --shell
```
#### Launch the default shell as the specified user, loading the user's environment and reading login-specific files (`.profile`, `.bash_profile`, etc.):
```shell
sudo --login --user={{user}}
```
#### List the allowed (and forbidden) commands for the invoking user:
```shell
sudo --list
```
{% endraw %}