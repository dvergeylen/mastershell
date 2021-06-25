---
layout: default
title: "gixy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gixy">
  <a href="/en/common/gixy.html">gixy</a> <a href="#gixy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analyze nginx configuration files.
> More information: <https://github.com/yandex/gixy>.

#### Analyze nginx configuration (default path: `/etc/nginx/nginx.conf`):
```shell
gixy
```
#### Analyze nginx configuration but skip specific tests:
```shell
gixy --skips {{http_splitting}}
```
#### Analyze nginx configuration with the specific severity level:
```shell
gixy {{-l|-ll|-lll}}
```
#### Analyze nginx configuration files on the specific path:
```shell
gixy {{path/to/configuration_file_1}} {{path/to/configuration_file_2}}
```
{% endraw %}