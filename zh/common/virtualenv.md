---
layout: default
title: "virtualenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virtualenv">
  <a href="/zh/common/virtualenv.html">virtualenv</a> <a href="#virtualenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建被隔离的的 Python 虚拟环境.
> 更多信息：<https://virtualenv.pypa.io/>.

#### 创建新环境:
```shell
virtualenv {{path/to/venv}}
```
#### 自定义提示符:
```shell
virtualenv --prompt={{prompt_prefix}} {{path/to/venv}}
```
#### 为虚拟环境使用不同的 Python 版本:
```shell
virtualenv --python={{path/to/pythonbin}} {{path/to/venv}}
```
#### 启动 （选择） 环境:
```shell
source {{path/to/venv}}/bin/activate
```
#### 停止环境:
```shell
deactivate
```
{% endraw %}