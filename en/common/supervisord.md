---
layout: default
title: "supervisord"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="supervisord">
  <a href="/en/common/supervisord.html">supervisord</a> <a href="#supervisord"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Supervisor is a client/server system for controlling some processes on UNIX-like operating systems.
> Supervisord is the server part of supervisor; it is primarily managed via a configuration file.
> More information: <http://supervisord.org>.

#### Start supervisord with specified configuration file:
```shell
supervisord -c {{path/to/file}}
```
#### Run supervisord in the foreground:
```shell
supervisord -n
```
{% endraw %}