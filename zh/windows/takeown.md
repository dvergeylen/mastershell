---
layout: default
title: "takeown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="takeown">
  <a href="/zh/windows/takeown.html">takeown</a> <a href="#takeown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 取得文件或目录的所有权.
> 更多信息: <https://docs.microsoft.com/windows-server/administration/windows-commands/takeown>.

#### 取得指定文件的所有权:
```shell
takeown /f {{路径/文件}}
```
#### 取得指定目录的所有权:
```shell
takeown /d {{路径/目录}}
```
#### 取得指定目录和所有子目录的所有权:
```shell
takeown /r /d {{路径/目录}}
```
#### 将所有权更改为管理员组，而不是当前用户:
```shell
takeown /a /f {{路径/文件}}
```
{% endraw %}