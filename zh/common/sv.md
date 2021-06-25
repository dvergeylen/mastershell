---
layout: default
title: "sv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sv">
  <a href="/zh/common/sv.html">sv</a> <a href="#sv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 控制正在运行的服务.
> 更多信息： <https://manpages.ubuntu.com/manpages/latest/man8/sv.8.html>.

#### 启动服务:
```shell
sudo sv up {{目标目录 / 服务文件}}
```
#### 停止服务:
```shell
sudo sv down {{目标目录 / 服务文件}}
```
#### 获取服务状态:
```shell
sudo sv status {{目标目录 / 服务文件}}
```
{% endraw %}