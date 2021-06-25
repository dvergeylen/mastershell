---
layout: default
title: "runsv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="runsv">
  <a href="/zh/common/runsv.html">runsv</a> <a href="#runsv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 启动和管理 runit 服务.
> 更多信息： <https://manpages.ubuntu.com/manpages/latest/man8/runsv.8.html>.

#### 以当前用户身份启动 runit 服务:
```shell
runsv {{目录 / 服务文件}}
```
#### 以 root 用户身份启动 runit 服务:
```shell
sudo runsv {{目录 / 服务文件}}
```
{% endraw %}