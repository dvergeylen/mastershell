---
layout: default
title: "heroku"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="heroku">
  <a href="/zh/common/heroku.html">heroku</a> <a href="#heroku"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从命令行创建和管理 Heroku 应用.
> 更多信息: <https://www.heroku.com/>.

#### 登录到你的 heroku 帐户:
```shell
heroku login
```
#### 创建一个 heroku 应用:
```shell
heroku create
```
#### 显示应用的日志:
```shell
heroku logs --app {{app_name}}
```
#### 在 dyno（Heroku 虚拟机）中运行一次性进程:
```shell
heroku run {{process_name}} --app {{app_name}}
```
#### 列出应用的 dyno（Heroku 虚拟机）:
```shell
heroku ps --app {{app_name}}
```
#### 永久销毁应用:
```shell
heroku destroy --app {{app_name}}
```
{% endraw %}