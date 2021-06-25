---
layout: default
title: "hexo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hexo">
  <a href="/en/common/hexo.html">hexo</a> <a href="#hexo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A fast, simple & powerful blog framework.
> More information: <https://hexo.io/>.

#### Initialize a website:
```shell
hexo init {{path/to/directory}}
```
#### Create a new article:
```shell
hexo new {{layout}} {{title}}
```
#### Generate static files:
```shell
hexo generate
```
#### Start a local server:
```shell
hexo server
```
#### Deploy the website:
```shell
hexo deploy
```
#### Clean the cache file (`db.json`) and generated files (`public/`):
```shell
hexo clean
```
{% endraw %}