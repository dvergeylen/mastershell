---
layout: default
title: "lolcat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lolcat">
  <a href="/en/common/lolcat.html">lolcat</a> <a href="#lolcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Put a rainbow in everything you `cat` to the console.
> More information: <https://github.com/busyloop/lolcat>.

#### Print a file to the console in rainbow colors:
```shell
lolcat {{path/to/file}}
```
#### Print the result of a text-producing command in rainbow colors:
```shell
{{fortune}} | lolcat
```
#### Print a file to the console with animated rainbow colors:
```shell
lolcat -a {{path/to/file}}
```
#### Print a file to the console with 24-bit (truecolor) rainbow colors:
```shell
lolcat -t {{path/to/file}}
```
{% endraw %}