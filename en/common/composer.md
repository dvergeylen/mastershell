---
layout: default
title: "composer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="composer">
  <a href="/en/common/composer.html">composer</a> <a href="#composer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A package-based dependency manager for PHP projects.
> More information: <https://getcomposer.org/>.

#### Interactively create a `composer.json` file:
```shell
composer init
```
#### Add a package as a dependency for this project, adding it to `composer.json`:
```shell
composer require {{user/package_name}}
```
#### Install all the dependencies in this project's `composer.json` and create `composer.lock`:
```shell
composer install
```
#### Uninstall a package from this project, removing it as a dependency from `composer.json`:
```shell
composer remove {{user/package_name}}
```
#### Update all the dependencies in this project's `composer.json` and note versions in `composer.lock` file:
```shell
composer update
```
#### Update composer lock only after updating `composer.json` manually:
```shell
composer update --lock
```
#### Learn more about why a dependency can't be installed:
```shell
composer why-not {{user/package_name}}
```
#### Update composer to its latest version:
```shell
composer self-update
```
{% endraw %}