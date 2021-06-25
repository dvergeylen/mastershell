---
layout: default
title: "bg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bg">
  <a href="/zh/common/bg.html">bg</a> <a href="#bg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 恢复被挂起的任务 (如. 使用 `Ctrl + Z`), 使它们在后台运行.
> 更多信息： <https://manned.org/bg>.

#### 恢复最近被挂起的任务，在后台运行:
```shell
bg
```
#### 恢复特定的任务 (使用 `jobs -l` 可以获取任务ID) 并在后台运行:
```shell
bg %{{job_id}}
```
{% endraw %}