---
layout: default
title: "sv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sv">
  <a href="/en/common/sv.html">sv</a> <a href="#sv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control a running runsv service.
> More information: <https://manpages.ubuntu.com/manpages/latest/man8/sv.8.html>.

#### Start a service:
```shell
sudo sv up {{path/to/service}}
```
#### Stop a service:
```shell
sudo sv down {{path/to/service}}
```
#### Get service status:
```shell
sudo sv status {{path/to/service}}
```
{% endraw %}