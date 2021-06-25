---
layout: default
title: "ansible-pull"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-pull">
  <a href="/en/common/ansible-pull.html">ansible-pull</a> <a href="#ansible-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pull ansible playbooks from a VCS repo and executes them for the local host.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-pull.html>.

#### Pull a playbook from a VCS and execute a default local.yml playbook:
```shell
ansible-pull -U {{repository_url}}
```
#### Pull a playbook from a VCS and execute a specific playbook:
```shell
ansible-pull -U {{repository_url}} {{playbook}}
```
#### Pull a playbook from a VCS at a specific branch and execute a specific playbook:
```shell
ansible-pull -U {{repository_url}} -C {{branch}} {{playbook}}
```
#### Pull a playbook from a VCS, specify hosts file and execute a specific playbook:
```shell
ansible-pull -U {{repository_url}} -i {{hosts_file}} {{playbook}}
```
{% endraw %}