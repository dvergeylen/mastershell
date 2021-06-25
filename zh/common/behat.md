---
layout: default
title: "behat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="behat">
  <a href="/zh/common/behat.html">behat</a> <a href="#behat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 基于Behaviour-Driven Development的自动化测试PHP框架
> 更多信息: <https://behat.org>.

#### 初始化一个PHP behat项目:
```shell
behat --init
```
#### 运行所有测试:
```shell
behat
```
#### 运行指定组所有的测试用例:
```shell
behat --suite={{组名}}
```
#### 运行所有测试，指定输入格式:
```shell
behat --format {{pretty|progress}}
```
#### 将测试结果输出到指定文件:
```shell
behat --out {{路径/到/文件}}
```
#### 展示测试组所在的目录清单:
```shell
behat --definitions
```
{% endraw %}