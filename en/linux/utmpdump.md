---
layout: default
title: "utmpdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="utmpdump">
  <a href="/en/linux/utmpdump.html">utmpdump</a> <a href="#utmpdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dump and load btmp, utmp and wtmp accounting files.

#### Dump the `/var/log/wtmp` file to the standard output as plain text:
```shell
utmpdump {{/var/log/wtmp}}
```
#### Load a previously dumped file into `/var/log/wtmp`:
```shell
utmpdump -r {{dumpfile}} > {{/var/log/wtmp}}
```
{% endraw %}