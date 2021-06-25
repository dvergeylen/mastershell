---
layout: default
title: "echo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="echo">
  <a href="/zh/common/echo.html">echo</a> <a href="#echo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 输出给定参数.
> 更多信息： <https://www.gnu.org/software/coreutils/echo>.

#### 输出文本信息. 注意: 引号是可选的:
```shell
echo "{{Hello World}}"
```
#### 输出带有环境变量的信息:
```shell
echo "{{My path is $PATH}}"
```
#### 打印不带尾随换行符的信息：
```shell
echo -n "{{Hello World}}"
```
#### 向文件添加信息:
```shell
echo "{{Hello World}}" >> {{file.txt}}
```
#### 启用反斜杠转义的解释（特殊字符）:
```shell
echo -e "{{Column 1\tColumn 2}}"
```
{% endraw %}