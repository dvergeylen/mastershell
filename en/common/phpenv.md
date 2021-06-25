---
layout: default
title: "phpenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpenv">
  <a href="/en/common/phpenv.html">phpenv</a> <a href="#phpenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP version manager for development purposes.
> More information: <https://github.com/phpenv/phpenv>.

#### Install a PHP version globally:
```shell
phpenv install {{version}}
```
#### Refresh shim files for all PHP binaries known to `phpenv`:
```shell
phpenv rehash
```
#### List all installed PHP versions:
```shell
phpenv versions
```
#### Display the currently active PHP version:
```shell
phpenv version
```
#### Set the global PHP version:
```shell
phpenv global {{version}}
```
#### Set the local PHP version, which overrides the global version:
```shell
phpenv local {{version}}
```
#### Unset the local PHP version:
```shell
phpenv local --unset
```
{% endraw %}