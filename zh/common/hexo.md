---
layout: default
title: "hexo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hexo">
  <a href="/zh/common/hexo.html">hexo</a> <a href="#hexo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 快速、简洁且高效的博客框架.
> 更多信息: <https://hexo.io/>.

#### 初始化一个网站:
```shell
hexo init {{path/to/directory}}
```
#### 创建一篇新文章:
```shell
hexo new {{layout}} {{title}}
```
#### 构建静态文件:
```shell
hexo generate
```
#### 启动本地服务器:
```shell
hexo server
```
#### 部署网站:
```shell
hexo deploy
```
#### 清理缓存文件 (`db.json`) 和生成的文件 (`public/`):
```shell
hexo clean
```
{% endraw %}