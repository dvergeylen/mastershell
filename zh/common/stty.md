---
layout: default
title: "stty"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stty">
  <a href="/zh/common/stty.html">stty</a> <a href="#stty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 设置终端设备接口的选项.
> 更多信息： <https://www.gnu.org/software/coreutils/stty>.

#### 显示当前终端的所有设置:
```shell
stty -a
```
#### 设置行数:
```shell
stty rows {{行数}}
```
#### 设置列数:
```shell
stty cols {{列数}}
```
#### 获取设备的实际传输速度:
```shell
stty -F {{目标 / 文件夹 / 驱动设备文件}} speed
```
#### 将当前终端的所有模式重置为合理值:
```shell
stty sane
```
{% endraw %}