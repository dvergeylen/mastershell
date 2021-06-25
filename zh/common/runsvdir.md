---
layout: default
title: "runsvdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="runsvdir">
  <a href="/zh/common/runsvdir.html">runsvdir</a> <a href="#runsvdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 运行整个目录下的服务.
> 更多信息： <https://manpages.ubuntu.com/manpages/latest/man8/runsvdir.8.html>.

#### 以当前用户身份启动和管理目录中的所有服务:
```shell
runsvdir {{目录 / 服务文件}}
```
#### 以 root 用户身份启动和管理目录中的所有服务:
```shell
sudo runsvdir {{目录 / 服务文件}}
```
#### 在单独会话中启动服务:
```shell
runsvdir -P {{目录 / 服务文件}}
```
{% endraw %}