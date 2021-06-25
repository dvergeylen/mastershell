---
layout: default
title: "more"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="more">
  <a href="/en/windows/more.html">more</a> <a href="#more"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display paginated output from stdin or a file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/more>.

#### Display paginated output from stdin:
```shell
{{echo test}} | more
```
#### Display paginated output from one or more files:
```shell
more {{path/to/file}}
```
#### Convert tabs to the specified number of spaces:
```shell
more {{path/to/file}} /t{{spaces}}
```
#### Clear the screen before displaying the page:
```shell
more {{path/to/file}} /c
```
#### Display the output starting at line 5:
```shell
more {{path/to/file}} +{{5}}
```
#### Enable extended interactive mode (see help for usage):
```shell
more {{path/to/file}} /e
```
#### Display full usage information:
```shell
more /?
```
{% endraw %}