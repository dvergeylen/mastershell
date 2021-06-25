---
layout: default
title: "ansible-playbook"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-playbook">
  <a href="/zh/common/ansible-playbook.html">ansible-playbook</a> <a href="#ansible-playbook"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 通过 SSH 协议在远程计算机上执行 playbook 中定义的任务.
> 主页：<https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html>.

#### 执行 playbook 中的任务:
```shell
ansible-playbook {{playbook}}
```
#### 在给定的主机清单文件中执行 playbook 中的命令:
```shell
ansible-playbook {{playbook}} -i {{清单文件}}
```
#### 通过定义在命令行中额外的变量执行 playbook 中的任务:
```shell
ansible-playbook {{playbook}} -e "{{变量 1}}={{值 1}} {{变量 2}}={{值 2}}"
```
#### 通过定义在一个 json 格式的文件中额外的变量执行 playbook 中的任务:
```shell
ansible-playbook {{playbook}} -e "@{{variables.json}}"
```
{% endraw %}