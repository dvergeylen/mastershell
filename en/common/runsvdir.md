---
layout: default
title: "runsvdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="runsvdir">
  <a href="/en/common/runsvdir.html">runsvdir</a> <a href="#runsvdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run an entire directory of services.
> More information: <https://manpages.ubuntu.com/manpages/latest/man8/runsvdir.8.html>.

#### Start and manage all services in a directory as the current user:
```shell
runsvdir {{path/to/services}}
```
#### Start and manage all services in a directory as root:
```shell
sudo runsvdir {{path/to/services}}
```
#### Start services in separate sessions:
```shell
runsvdir -P {{path/to/services}}
```
{% endraw %}