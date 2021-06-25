---
layout: default
title: "ansible-inventory"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-inventory">
  <a href="/en/common/ansible-inventory.html">ansible-inventory</a> <a href="#ansible-inventory"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or dump an Ansible inventory.
> See also: `ansible`.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-inventory.html>.

#### Display the default inventory:
```shell
ansible-inventory --list
```
#### Display a custom inventory:
```shell
ansbile-inventory --list --inventory {{path/to/file_or_script_or_directory}}
```
#### Display the default inventory in YAML:
```shell
ansible-inventory --list --yaml
```
#### Dump the default inventory to a file:
```shell
ansible-inventory --list --output {{path/to/file}}
```
{% endraw %}