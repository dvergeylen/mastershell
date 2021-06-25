---
layout: default
title: "phan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phan">
  <a href="/en/common/phan.html">phan</a> <a href="#phan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A static analysis tool for PHP.
> More information: <https://github.com/phan/phan>.

#### Generate a `.phan/config.php` in the current directory:
```shell
phan --init
```
#### Generate a Phan configuration file using a specific level (1 being strictest to 5 being the least strict):
```shell
phan --init --init-level {{level}}
```
#### Analyse the current directory:
```shell
phan
```
#### Analyse one or more directories:
```shell
phan --directory {{path/to/directory}} --directory {{path/to/another_directory}}
```
#### Specify a config file (defaults to `.phan/config.php`):
```shell
phan --config-file {{path/to/config.php}}
```
#### Specify the output mode:
```shell
phan --output-mode {{text|verbose|json|csv|codeclimate|checkstyle|pylint|html}}
```
#### Specify the number of parallel processes:
```shell
phan --processes {{number_of_processes}}
```
{% endraw %}