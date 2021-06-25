---
layout: default
title: "xtrlock"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xtrlock">
  <a href="/en/linux/xtrlock.html">xtrlock</a> <a href="#xtrlock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lock the X display until the user supplies their password.

#### Lock the display and show a padlock instead of the cursor:
```shell
xtrlock
```
#### Display a blank screen as well as the padlock cursor:
```shell
xtrlock -b
```
#### Fork the xtrlock process and return immediately:
```shell
xtrlock -f
```
{% endraw %}