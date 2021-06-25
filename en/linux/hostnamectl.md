---
layout: default
title: "hostnamectl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hostnamectl">
  <a href="/en/linux/hostnamectl.html">hostnamectl</a> <a href="#hostnamectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get or set the hostname of the computer.

#### Get the hostname of the computer:
```shell
hostnamectl
```
#### Set the hostname of the computer:
```shell
sudo hostnamectl set-hostname "{{hostname}}"
```
#### Set a pretty hostname for the computer:
```shell
sudo hostnamectl set-hostname --static "{{hostname.example.com}}" && sudo hostnamectl set-hostname --pretty "{{hostname}}"
```
#### Reset hostname to its default value:
```shell
sudo hostnamectl set-hostname --pretty ""
```
{% endraw %}