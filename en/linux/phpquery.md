---
layout: default
title: "phpquery"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpquery">
  <a href="/en/linux/phpquery.html">phpquery</a> <a href="#phpquery"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PHP extension manager for Debian-based OSes.

#### List available PHP versions:
```shell
sudo phpquery -V
```
#### List available SAPIs for PHP 7.3:
```shell
sudo phpquery -v {{7.3}} -S
```
#### List enabled extensions for PHP 7.3 with the cli SAPI:
```shell
sudo phpquery -v {{7.3}} -s {{cli}} -M
```
#### Check if the json extension is enabled for PHP 7.3 with the apache2 SAPI:
```shell
sudo phpquery -v {{7.3}} -s {{apache2}} -m {{json}}
```
{% endraw %}