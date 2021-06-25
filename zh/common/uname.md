---
layout: default
title: "uname"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uname">
  <a href="/zh/common/uname.html">uname</a> <a href="#uname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 输出关于当前机器和运行在该机器上的操作系统的详细信息。
> 注意：如需了解操作系统的其他信息，请尝试使用 `lsb_release` 命令。
> 更多信息： <https://www.gnu.org/software/coreutils/uname>.

#### 打印硬件相关信息：机器和处理器：
```shell
uname -mp
```
#### 打印软件相关信息：操作系统、发行号和版本：
```shell
uname -srv
```
#### 打印系统的名称（主机名）：
```shell
uname -n
```
#### 打印所有可用的系统信息（硬件、软件、名称）：
```shell
uname -a
```
{% endraw %}