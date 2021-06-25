---
layout: default
title: "a2query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2query">
  <a href="/en/linux/a2query.html">a2query</a> <a href="#a2query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retrieve runtime configuration from Apache on Debian-based OSes.
> More information: <https://manpages.debian.org/buster/apache2/a2query.1.en.html>.

#### List enabled Apache modules:
```shell
sudo a2query -m
```
#### Check if a specific module is installed:
```shell
sudo a2query -m {{module_name}}
```
#### List enabled virtual hosts:
```shell
sudo a2query -s
```
#### Display the currently enabled Multi Processing Module:
```shell
sudo a2query -M
```
#### Display the Apache version:
```shell
sudo a2query -v
```
{% endraw %}