---
layout: default
title: "ansible-galaxy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-galaxy">
  <a href="/zh/common/ansible-galaxy.html">ansible-galaxy</a> <a href="#ansible-galaxy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建和管理 Ansible 角色.
> 主页：<https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html>.

#### 安装一个角色:
```shell
ansible-galaxy install {{用户名.角色名}}
```
#### 移除一个角色:
```shell
ansible-galaxy remove {{用户名.角色名}}
```
#### 列出已安装的角色:
```shell
ansible-galaxy list
```
#### 搜索一个指定的角色:
```shell
ansible-galaxy search {{角色名}}
```
#### 创建一个新的角色:
```shell
ansible-galaxy init {{角色名}}
```
{% endraw %}