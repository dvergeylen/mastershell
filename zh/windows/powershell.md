---
layout: default
title: "powershell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="powershell">
  <a href="/zh/windows/powershell.html">powershell</a> <a href="#powershell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 专为系统管理而设计的命令行 shell 和脚本语言.
> 更多信息: <https://docs.microsoft.com/windows-server/administration/windows-commands/powershell>.

#### 在命令提示符窗口中启动 Windows PowerShell 会话:
```shell
powershell
```
#### 加载一个特定的 PowerShell 控制台文件:
```shell
powershell -PSConsoleFile {{路径/file}}
```
#### 用指定版本的 PowerShell 启动会话:
```shell
powershell -Version {{版本}}
```
#### 防止运行启动命令后 shell 退出:
```shell
powershell -NoExit
```
#### 描述发送到 PowerShell 的数据格式:
```shell
powershell -InputFormat {{Text|XML}}
```
#### 设定 PowerShell 输出的格式:
```shell
powershell -OutputFormat {{Text|XML}}
```
#### 显示帮助:
```shell
powershell -Help
```
{% endraw %}