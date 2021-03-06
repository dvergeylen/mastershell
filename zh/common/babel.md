---
layout: default
title: "babel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="babel">
  <a href="/zh/common/babel.html">babel</a> <a href="#babel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一款JavaScript的编译器，将下一代ES语法转换为兼容语法。
> 更多信息: <https://babeljs.io/>.

#### 转编译指定文件到标准输出:
```shell
babel {{路径/到/文件}}
```
#### 转编译指定文件，输入为特定文件:
```shell
babel {{路径/到/输入文件}} --out-file {{路径/到/输出文件}}
```
#### 监听文件变动触发转编译:
```shell
babel {{路径/到/输入文件}} --watch
```
#### 转编译整个目录下的js文件:
```shell
babel {{路径/到/输入文件目录}}
```
#### 跳过指定目录下指定文件的编译（多文件使用英文逗号“,”分隔）:
```shell
babel {{路径/到/输入文件目录}} --ignore {{被忽略文件}}
```
#### 转编译后，执行压缩:
```shell
babel {{路径/到/输入文件}} --minified
```
#### 使用预设值:
```shell
babel {{路径/到/输入文件}} --presets {{预设项}}
```
{% endraw %}