---
layout: default
title: "node"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="node">
  <a href="/zh/common/node.html">node</a> <a href="#node"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 服务器后端 JavaScript 平台 (Node.js).
> 更多信息: <https://nodejs.org>.

#### 运行一个 JavaScript 文件:
```shell
node {{文件名}}
```
#### 开始一个 REPL 交互式解释器:
```shell
node
```
#### 执行输入的 JavaScript 代码:
```shell
node -e "{{代码}}"
```
#### 执行输入的 JavaScript 代码并显示结果:
```shell
node -p "{{代码}}"
```
#### 启动检查器并在程序源码解析完成后等待调试器连接:
```shell
node --no-lazy --inspect-brk {{文件名}}
```
{% endraw %}