---
layout: default
title: "apachectl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apachectl">
  <a href="/en/osx/apachectl.html">apachectl</a> <a href="#apachectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache HTTP Server control interface for macOS.

#### Start the `org.apache.httpd` launchd job:
```shell
apachectl start
```
#### Stop the launchd job:
```shell
apachectl stop
```
#### Stop, then start launchd job:
```shell
apachectl restart
```
{% endraw %}