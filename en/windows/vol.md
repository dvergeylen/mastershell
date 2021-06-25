---
layout: default
title: "vol"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vol">
  <a href="/en/windows/vol.html">vol</a> <a href="#vol"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about volumes.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/vol>.

#### Display the label and serial number for the current drive:
```shell
vol
```
#### Display the label and serial number for a specific volume:
```shell
vol {{D:}}
```
{% endraw %}