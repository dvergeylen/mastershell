---
layout: default
title: "runsv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="runsv">
  <a href="/en/common/runsv.html">runsv</a> <a href="#runsv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Start and manage a runit service.
> More information: <https://manpages.ubuntu.com/manpages/latest/man8/runsv.8.html>.

#### Start a runit service as the current user:
```shell
runsv {{path/to/service}}
```
#### Start a runit service as root:
```shell
sudo runsv {{path/to/service}}
```
{% endraw %}