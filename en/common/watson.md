---
layout: default
title: "watson"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="watson">
  <a href="/en/common/watson.html">watson</a> <a href="#watson"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A wonderful CLI to track your time.
> More information: <https://github.com/TailorDev/Watson>.

#### Start monitoring time in project:
```shell
watson start {{project}}
```
#### Start monitoring time in project with tags:
```shell
watson start {{project}} +{{tag}}
```
#### Stop monitoring time for the current project:
```shell
watson stop
```
#### Display latest working sessions:
```shell
watson log
```
#### Edit most recent frame:
```shell
watson edit
```
#### Remove most recent frame:
```shell
watson remove
```
{% endraw %}