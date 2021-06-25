---
layout: default
title: "fuser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fuser">
  <a href="/en/linux/fuser.html">fuser</a> <a href="#fuser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display process IDs currently using files or sockets.

#### Find which processes are accessing a file or directory:
```shell
fuser {{path/to/file_or_directory}}
```
#### Show more fields (`USER`, `PID`, `ACCESS` and `COMMAND`):
```shell
fuser --verbose {{path/to/file_or_directory}}
```
#### Identify processes using a TCP socket:
```shell
fuser --namespace tcp {{port}}
```
#### Kill all processes accessing a file or directory (sends the `SIGKILL` signal):
```shell
fuser --kill {{path/to/file_or_directory}}
```
#### Find which processes are accessing the filesystem containing a specific file or directory:
```shell
fuser --mount {{path/to/file_or_directory}}
```
{% endraw %}