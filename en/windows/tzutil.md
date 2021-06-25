---
layout: default
title: "tzutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tzutil">
  <a href="/en/windows/tzutil.html">tzutil</a> <a href="#tzutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for displaying or configuring the system time zone.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/tzutil>.

#### Get the current time zone:
```shell
tzutil /g
```
#### Display a list of available time zones:
```shell
tzutil /l
```
#### Set the system time zone to the specific value:
```shell
tzutil /s {{timezone_id}}
```
{% endraw %}