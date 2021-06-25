---
layout: default
title: "php yii"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="php-yii">
  <a href="/en/common/php-yii.html">php yii</a> <a href="#php-yii"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yii Framework's command-line interface.
> More information: <https://yiiframework.com>.

#### Display a list of all available commands:
```shell
php yii {{help}}
```
#### Start PHP's built-in web server for the current Yii application:
```shell
php yii {{serve}}
```
#### Generate a controller, views and related files for the CRUD actions on the specified model class:
```shell
php yii {{gii/crud}} --modelClass={{ModelName}} --controllerClass={{ControllerName}}
```
{% endraw %}