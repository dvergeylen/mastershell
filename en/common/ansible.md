---
layout: default
title: "ansible"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible">
  <a href="/en/common/ansible.html">ansible</a> <a href="#ansible"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage groups of computers remotely over SSH.
> Use the `/etc/ansible/hosts` file to add new groups/hosts.
> More information: <https://www.ansible.com/>.

#### List hosts belonging to a group:
```shell
ansible {{group}} --list-hosts
```
#### Ping a group of hosts by invoking the ping module:
```shell
ansible {{group}} -m ping
```
#### Display facts about a group of hosts by invoking the setup module:
```shell
ansible {{group}} -m setup
```
#### Execute a command on a group of hosts by invoking command module with arguments:
```shell
ansible {{group}} -m command -a '{{my_command}}'
```
#### Execute a command with administrative privileges:
```shell
ansible {{group}} --become --ask-become-pass -m command -a '{{my_command}}'
```
#### Execute a command using a custom inventory file:
```shell
ansible {{group}} -i {{inventory_file}} -m command -a '{{my_command}}'
```
#### List the groups in an inventory:
```shell
ansible localhost -m debug -a '{{var=groups.keys()}}'
```
{% endraw %}