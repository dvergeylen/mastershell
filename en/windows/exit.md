---
layout: default
title: "exit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exit">
  <a href="/en/windows/exit.html">exit</a> <a href="#exit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Quit the current CMD instance or the current batch file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/exit>.

#### Quit the current CMD instance:
```shell
exit
```
#### Quit the current batch script:
```shell
exit /b
```
#### Quit using a specific exit code:
```shell
exit {{exit_code}}
```
{% endraw %}