---
layout: default
title: "gh repo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-repo">
  <a href="/zh/common/gh-repo.html">gh repo</a> <a href="#gh-repo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在命令行上操作 GitHub 仓库.
> 更多信息: <https://cli.github.com/manual/gh_repo>.

#### 创建一个新的仓库(如果没有设置仓库名称，默认将为当前目录的名称):
```shell
gh repo create {{名称}}
```
#### 克隆一个仓库:
```shell
gh repo clone {{拥有者}}/{{仓库}}
```
#### 复刻并克隆一个仓库:
```shell
gh repo fork {{拥有者}}/{{仓库}} --clone
```
#### 在网络浏览器中查看仓库:
```shell
gh repo view {{仓库}} --web
```
{% endraw %}