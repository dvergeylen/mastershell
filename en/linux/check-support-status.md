---
layout: default
title: "check-support-status"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="check-support-status">
  <a href="/en/linux/check-support-status.html">check-support-status</a> <a href="#check-support-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Identify installed Debian packages for which support has had to be limited or prematurely ended.
> More information: <https://manpages.debian.org/buster/debian-security-support/check-support-status.1.en.html>.

#### Display packages whose support is limited, has already ended or will end earlier than the distribution's end of life:
```shell
check-support-status
```
#### Display only packages whose support has ended:
```shell
check-support-status --type {{ended}}
```
#### Skip printing a headline:
```shell
check-support-status --no-heading
```
{% endraw %}