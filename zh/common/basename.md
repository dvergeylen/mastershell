---
layout: default
title: "basename"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="basename">
  <a href="/zh/common/basename.html">basename</a> <a href="#basename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 移除一个路径的目录部分字符.
> 更多信息： <https://www.gnu.org/software/coreutils/basename>.

#### 仅显示文件名:
```shell
basename {{路径/到/文件}}
```
#### 显示路径字符最右边表示目录的字符:
```shell
basename {{路径/到/目录/}}
```
#### 展示无后缀的文件名称:
```shell
basename {{路径/到/文件}} {{后缀}}
```
{% endraw %}