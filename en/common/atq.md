---
layout: default
title: "atq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atq">
  <a href="/en/common/atq.html">atq</a> <a href="#atq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show jobs scheduled by `at` or `batch` commands.
> More information: <https://man.archlinux.org/man/at.1>.

#### Show the current user's scheduled jobs:
```shell
atq
```
#### Show jobs from queue named 'a' (queues have single-character names):
```shell
atq -q {{a}}
```
#### Show jobs of all users (run as super user):
```shell
sudo atq
```
{% endraw %}