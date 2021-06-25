---
layout: default
title: "useradd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="useradd">
  <a href="/en/linux/useradd.html">useradd</a> <a href="#useradd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a new user.
> More information: <https://manned.org/useradd>.

#### Create new user:
```shell
useradd {{name}}
```
#### Create new user with a default home directory:
```shell
useradd --create-home {{name}}
```
#### Create new user with specified shell:
```shell
useradd --shell {{path/to/shell}} {{name}}
```
#### Create new user belonging to additional groups (mind the lack of whitespace):
```shell
useradd --groups {{group1,group2}} {{name}}
```
#### Create new system user without a home directory:
```shell
useradd --no-create-home --system {{name}}
```
{% endraw %}