---
layout: default
title: "ifup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ifup">
  <a href="/en/linux/ifup.html">ifup</a> <a href="#ifup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool used to enable network interfaces.
> More information: <https://manpages.debian.org/latest/ifupdown/ifup.8.html>.

#### Enable interface eth0:
```shell
ifup {{eth0}}
```
#### Enable all the interfaces defined with "auto" in `/etc/network/interfaces`:
```shell
ifup -a
```
{% endraw %}