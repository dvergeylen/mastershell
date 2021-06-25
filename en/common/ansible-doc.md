---
layout: default
title: "ansible-doc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-doc">
  <a href="/en/common/ansible-doc.html">ansible-doc</a> <a href="#ansible-doc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information on modules installed in Ansible libraries.
> Display a terse listing of plugins and their short descriptions.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-doc.html>.

#### List available action plugins (modules):
```shell
ansible-doc --list
```
#### List available plugins of a specific type:
```shell
ansible-doc --type {{plugin_type}} --list
```
#### Show information about a specific action plugin (module):
```shell
ansible-doc {{plugin_name}}
```
#### Show information about a plugin with a specific type:
```shell
ansible-doc --type {{plugin_type}} {{plugin_name}}
```
#### Show the playbook snippet for action plugin (modules):
```shell
ansible-doc --snippet {{plugin_name}}
```
#### Show information about an action plugin (module) as JSON:
```shell
ansible-doc --json {{plugin_name}}
```
{% endraw %}