---
layout: default
title: "act"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="act">
  <a href="/zh/common/act.html">act</a> <a href="#act"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用Docker本地运行GitHub Actions
> 更多信息: <https://github.com/nektos/act>.

#### 列出可用的actions清单:
```shell
act -l
```
#### 运行默认event:
```shell
act
```
#### 运行指定event:
```shell
act {{事件类型}}
```
#### 运行指定action:
```shell
act -a {{action_id}}
```
#### 非实际运行actions (也就是dry-run模式):
```shell
act -n
```
#### 展示详细记录:
```shell
act -v
```
{% endraw %}