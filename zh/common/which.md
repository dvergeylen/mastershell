---
layout: default
title: "which"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="which">
  <a href="/zh/common/which.html">which</a> <a href="#which"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在用户的`PATH`中寻找可执行文件的路径

#### 在`PATH`中寻找可执行文件并打印第一个匹配的结果:
```shell
which {{executable}}
```
#### 如果有多个匹配结果则打印所有结果:
```shell
which -a {{executable}}
```
{% endraw %}