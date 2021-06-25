---
layout: default
title: "yarn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yarn">
  <a href="/zh/common/yarn.html">yarn</a> <a href="#yarn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> JavaScript 和 Node.js package manager 的一个替代.
> 更多信息：<https://yarnpkg.com>.

#### 全局安装一个模块:
```shell
yarn global add {{module_name}}
```
#### 安装 `package.json` 中指定的依赖 (`install` 命令是可选的 -- 你可以直接输入`yarn`):
```shell
yarn install
```
#### 安装一个模块并将其写入 `package.json` 中的依赖项 （增加 `--dev` 来作为开发依赖写入）:
```shell
yarn add {{module_name}}@{{version}}
```
#### 卸载一个模块并将其从 `package.json` 的依赖项中移除:
```shell
yarn remove {{module_name}}
```
#### 交互式地创建一个 `package.json` 文件:
```shell
yarn init
```
#### 确认一个模块是否是一个依赖项并且列出依赖其的模块:
```shell
yarn why {{module_name}}
```
{% endraw %}