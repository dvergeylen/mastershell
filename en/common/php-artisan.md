---
layout: default
title: "php artisan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="php-artisan">
  <a href="/en/common/php-artisan.html">php artisan</a> <a href="#php-artisan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Laravel's Artisan command-line interface.
> More information: <https://laravel.com/docs/artisan>.

#### Start PHP's built-in web server for the current Laravel application:
```shell
php artisan serve
```
#### Start an interactive PHP command-line interface:
```shell
php artisan tinker
```
#### Generate a new Eloquent model class with a migration, factory and resource controller:
```shell
php artisan make:model {{ModelName}} --all
```
#### Display a list of all available commands:
```shell
php artisan help
```
{% endraw %}