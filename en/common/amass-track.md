---
layout: default
title: "amass track"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="amass-track">
  <a href="/en/common/amass-track.html">amass track</a> <a href="#amass-track"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Track differences between enumerations of the same domain.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-track-subcommand>.

#### Show the difference between the last two enumerations of the specified domain:
```shell
amass track -dir {{path/to/database_directory}} -d {{domain_name}} -last 2
```
#### Show the difference between a certain point in time and the last enumeration:
```shell
amass track -dir {{path/to/database_directory}} -d {{domain_name}} -since {{01/02 15:04:05 2006 MST}}
```
{% endraw %}