---
layout: default
title: "color"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="color">
  <a href="/en/windows/color.html">color</a> <a href="#color"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set the console foreground and background colors.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/color>.

#### Set the console colors to the default values:
```shell
color
```
#### List available color values and detailed information:
```shell
color /?
```
#### Set the console foreground and background to a specific color:
```shell
color {{foreground_code}}{{background_code}}
```
{% endraw %}