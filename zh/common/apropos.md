---
layout: default
title: "apropos"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apropos">
  <a href="/zh/common/apropos.html">apropos</a> <a href="#apropos"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 manpages 中搜索，例如查找一个新命令.
> 更多信息： <https://manned.org/apropos>.

#### 搜索关键字:
```shell
apropos {{正则表达式}}
```
#### 搜索时不限制输出到终端宽度:
```shell
apropos -l {{正则表达式}}
```
{% endraw %}