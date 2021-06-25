---
layout: default
title: "clip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clip">
  <a href="/en/windows/clip.html">clip</a> <a href="#clip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy input content to the Windows clipboard.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/clip>.

#### Pipe command-line output to the Windows clipboard:
```shell
{{dir}} | clip
```
#### Copy the contents of a file to the Windows clipboard:
```shell
clip < {{path/to/file.ext}}
```
#### Copy text with a trailing newline to the Windows clipboard:
```shell
echo {{some text}} | clip
```
#### Copy text without a trailing newline to the Windows clipboard:
```shell
echo | set /p="some text" | clip
```
{% endraw %}