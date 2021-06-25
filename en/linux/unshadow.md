---
layout: default
title: "unshadow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unshadow">
  <a href="/en/linux/unshadow.html">unshadow</a> <a href="#unshadow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility provided by the John the Ripper project to obtain the traditional Unix password file if the system uses shadow passwords.
> More information: <https://www.openwall.com/john/>.

#### Combine the `/etc/shadow` and `/etc/passwd` of the current system:
```shell
sudo unshadow /etc/passwd /etc/shadow
```
#### Combine two arbitrary shadow and password files:
```shell
sudo unshadow {{path/to/passwd}} {{path/to/shadow}}
```
{% endraw %}