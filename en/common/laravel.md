---
layout: default
title: "laravel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="laravel">
  <a href="/en/common/laravel.html">laravel</a> <a href="#laravel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line installer for the Laravel framework.
> More information: <https://laravel.com>.

#### Create a new Laravel application:
```shell
laravel new {{name}}
```
#### Use the latest development release:
```shell
laravel new {{name}} --dev
```
#### Overwrite if the directory already exists:
```shell
laravel new {{name}} --force
```
#### Install the Laravel Jetstream scaffolding:
```shell
laravel new {{name}} --jet
```
#### Install the Laravel Jetstream scaffolding with a specific stack:
```shell
laravel new {{name}} --jet --stack {{livewire|inertia}}
```
#### Install the Laravel Jetstream scaffolding with support for teams:
```shell
laravel new {{name}} --jet --teams
```
#### List the available installer commands:
```shell
laravel list
```
{% endraw %}