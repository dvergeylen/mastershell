---
layout: default
title: "ssh-add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-add">
  <a href="/zh/osx/ssh-add.html">ssh-add</a> <a href="#ssh-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 ssh 代理中管理加载的 ssh 密钥.
> 需要确保 ssh 代理已启动并正在运行以加载其中的密钥.

#### 将 `~/.ssh` 中的默认 ssh 密钥添加到 `ssh` 代理:
```shell
ssh-add
```
#### 向 ssh 代理添加指定密钥:
```shell
ssh-add {{目录 / 私钥文件}}
```
#### 列出当前加载的密钥的指纹:
```shell
ssh-add -l
```
#### 从 ssh 代理中删除密钥:
```shell
ssh-add -d {{目录 / 私钥文件}}
```
#### 从 ssh 代理中删除所有当前已有的密钥:
```shell
ssh-add -D
```
#### 向 ssh 代理和密钥链添加密钥:
```shell
ssh-add -K {{目录 / 私钥文件}}
```
{% endraw %}