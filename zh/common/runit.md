---
layout: default
title: "runit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="runit">
  <a href="/zh/common/runit.html">runit</a> <a href="#runit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 三级初始化系统.
> 更多信息： <https://wiki.archlinux.org/index.php/Runit>.

#### 启动 runit 的三阶段初始化方案:
```shell
runit
```
#### 停止运行 runit:
```shell
kill --CONT {{runit 进程 id}}
```
{% endraw %}