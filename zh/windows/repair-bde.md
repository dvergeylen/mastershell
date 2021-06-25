---
layout: default
title: "repair-bde"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="repair-bde">
  <a href="/zh/windows/repair-bde.html">repair-bde</a> <a href="#repair-bde"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 尝试修复或解密损坏的 BitLocker 加密卷.

#### 尝试修复一个指定的卷:
```shell
repair-bde {{C:}}
```
#### 尝试修复指定的卷并输出到另一个卷:
```shell
repair-bde {{C:}} {{D:}}
```
#### 尝试使用提供的恢复密钥文件修复指定的卷:
```shell
repair-bde {{C:}} -RecoveryKey {{bek 文件的路径}}
```
#### 尝试使用提供的数字恢复密码修复指定的卷:
```shell
repair-bde {{C:}} -RecoveryPassword {{密码}}
```
#### 尝试使用提供的密码修复指定的卷:
```shell
repair-bde {{C:}} -Password {{密码}}
```
#### 尝试使用提供的密钥包修复指定的卷:
```shell
repair-bde {{C:}} -KeyPackage {{目录的路径}}
```
#### 将日志输出到指定的文件:
```shell
repair-bde {{C:}} -LogFile {{文件的路径}}
```
#### 显示所有可用的选项:
```shell
repair-bde /?
```
{% endraw %}