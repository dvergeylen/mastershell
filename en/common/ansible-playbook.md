---
layout: default
title: "ansible-playbook"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-playbook">
  <a href="/en/common/ansible-playbook.html">ansible-playbook</a> <a href="#ansible-playbook"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute tasks defined in playbook on remote machines over SSH.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html>.

#### Run tasks in playbook:
```shell
ansible-playbook {{playbook}}
```
#### Run tasks in playbook with custom host inventory:
```shell
ansible-playbook {{playbook}} -i {{inventory_file}}
```
#### Run tasks in playbook with extra variables defined via the command-line:
```shell
ansible-playbook {{playbook}} -e "{{variable1}}={{value1}} {{variable2}}={{value2}}"
```
#### Run tasks in playbook with extra variables defined in a json file:
```shell
ansible-playbook {{playbook}} -e "@{{variables.json}}"
```
#### Run tasks in playbook for the given tags:
```shell
ansible-playbook {{playbook}} --tags {{tag1,tag2}}
```
#### Run tasks in a playbook starting at a specific task:
```shell
ansible-playbook {{playbook}} --start-at {{task_name}}
```
{% endraw %}