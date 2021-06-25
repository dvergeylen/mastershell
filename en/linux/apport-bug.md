---
layout: default
title: "apport-bug"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apport-bug">
  <a href="/en/linux/apport-bug.html">apport-bug</a> <a href="#apport-bug"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> File a bug report on Ubuntu.
> More information: <https://wiki.ubuntu.com/Apport>.

#### Report a bug about the whole system:
```shell
apport-bug
```
#### Report a bug about a specific package:
```shell
apport-bug {{package}}
```
#### Report a bug about a specific executable:
```shell
apport-bug {{path/to/executable}}
```
#### Report a bug about a specific process:
```shell
apport-bug {{PID}}
```
{% endraw %}