---
layout: default
title: "vagrant"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vagrant">
  <a href="/en/common/vagrant.html">vagrant</a> <a href="#vagrant"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage lightweight, reproducible, and portable development environments.
> More information: <https://www.vagrantup.com>.

#### Create Vagrantfile in current directory with the base Vagrant box:
```shell
vagrant init
```
#### Create Vagrantfile with the Ubuntu 14.04 (Trusty Tahr) box from HashiCorp Atlas:
```shell
vagrant init ubuntu/trusty32
```
#### Start and provision the vagrant environment:
```shell
vagrant up
```
#### Suspend the machine:
```shell
vagrant suspend
```
#### Halt the machine:
```shell
vagrant halt
```
#### Connect to machine via SSH:
```shell
vagrant ssh
```
#### Output the SSH configuration file of the running Vagrant machine:
```shell
vagrant ssh-config
```
{% endraw %}