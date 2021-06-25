---
layout: default
title: "ansible-galaxy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-galaxy">
  <a href="/en/common/ansible-galaxy.html">ansible-galaxy</a> <a href="#ansible-galaxy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manage Ansible roles.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html>.

#### Install a role:
```shell
ansible-galaxy install {{username.role_name}}
```
#### Remove a role:
```shell
ansible-galaxy remove {{username.role_name}}
```
#### List installed roles:
```shell
ansible-galaxy list
```
#### Search for a given role:
```shell
ansible-galaxy search {{role_name}}
```
#### Create a new role:
```shell
ansible-galaxy init {{role_name}}
```
{% endraw %}