---
layout: default
title: "buku"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="buku">
  <a href="/zh/common/buku.html">buku</a> <a href="#buku"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 命令行版本的书签管理器.
> 更多信息: <https://github.com/jarun/Buku>.

#### 根据关键词和标签查找书签:
```shell
buku {{关键字}} --stag {{标签}}
```
#### 添加书签，并且打上标签:
```shell
buku --add {{https://example.com}} {{搜索引擎}}, {{标签}}
```
#### 删除一个书签:
```shell
buku --delete {{书签id}}
```
#### 打开编辑器，修改书签:
```shell
buku --write {{书签id}}
```
#### 将指定标签移除:
```shell
buku --update {{书签id}} --tag {{-}} {{搜索引擎}}
```
{% endraw %}