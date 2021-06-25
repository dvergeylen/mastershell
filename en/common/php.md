---
layout: default
title: "php"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="php">
  <a href="/en/common/php.html">php</a> <a href="#php"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PHP command-line interface.
> More information: <https://php.net>.

#### Parse and execute a php script:
```shell
php {{file}}
```
#### Check syntax on (i.e. lint) a PHP script:
```shell
php -l {{file}}
```
#### Run PHP interactively:
```shell
php -a
```
#### Run PHP code (Notes: Don't use <? ?> tags; escape double quotes with backslash):
```shell
php -r "{{code}}"
```
#### Start a PHP built-in web server in the current directory:
```shell
php -S {{host:port}}
```
#### Get a list of installed PHP extensions:
```shell
php -m
```
#### Display information about the current PHP configuration:
```shell
php -i
```
{% endraw %}