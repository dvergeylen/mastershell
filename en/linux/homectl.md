---
layout: default
title: "homectl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="homectl">
  <a href="/en/linux/homectl.html">homectl</a> <a href="#homectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, remove, change or inspect home directories using the systemd-homed service.
> More information: <https://man.archlinux.org/man/homectl.1>.

#### List user accounts and their associated home directories:
```shell
homectl list
```
#### Create a user account and their associated home directory:
```shell
sudo homectl create {{username}}
```
#### Remove a specific user and the associated home directory:
```shell
sudo homectl remove {{username}}
```
#### Change the password for a specific user:
```shell
sudo homectl passwd {{username}}
```
#### Run a shell or a command with access to a specific home directory:
```shell
sudo homectl with {{username}} -- {{command}} {{command_arguments}}
```
#### Lock or unlock a specific home directory:
```shell
sudo homectl {{lock|unlock}} {{username}}
```
#### Change the disk space assigned to a specific home directory to 100 GiB:
```shell
sudo homectl resize {{username}} {{100G}}
```
#### Display help:
```shell
homectl --help
```
{% endraw %}