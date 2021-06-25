---
layout: default
title: "caffeinate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="caffeinate">
  <a href="/en/osx/caffeinate.html">caffeinate</a> <a href="#caffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prevent mac from sleeping.

#### Prevent from sleeping for 1 hour (3600 seconds):
```shell
caffeinate -u -t {{3600}}
```
#### Prevent from sleeping until a command completes:
```shell
caffeinate -s {{command}}
```
#### Prevent from sleeping until you type Ctrl-C:
```shell
caffeinate -i
```
{% endraw %}