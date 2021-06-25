---
layout: default
title: "mkswap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkswap">
  <a href="/en/linux/mkswap.html">mkswap</a> <a href="#mkswap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sets up a Linux swap area on a device or in a file.

#### Setup a given partition as swap area:
```shell
sudo mkswap {{/dev/sdb7}}
```
#### Use a given file as swap area:
```shell
sudo mkswap {{path/to/file}}
```
#### Check a partition for bad blocks before creating the swap area:
```shell
sudo mkswap -c {{/dev/sdb7}}
```
#### Specify a label for the file (to allow `swapon` to use the label):
```shell
sudo mkswap -L {{swap1}} {{path/to/file}}
```
{% endraw %}