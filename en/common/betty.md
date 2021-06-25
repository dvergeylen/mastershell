---
layout: default
title: "betty"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="betty">
  <a href="/en/common/betty.html">betty</a> <a href="#betty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Use natural language to execute commands.
> More information: <https://github.com/pickhardt/betty>.

#### Ask Betty something:
```shell
betty {{what time is it}}
```
#### Ask Betty version:
```shell
betty version
```
#### Download a file:
```shell
betty download {{https://example.com/file.png}} to {{file.png}}
```
#### Compress a file or directory to one of the support archive formats:
```shell
betty {{zip}} {{path/to/file_or_directory}}
```
#### Extract an archive into the current directory:
```shell
betty {{unzip}} {{archive.tar.gz}}
```
#### Extract an archive into a directory:
```shell
betty unarchive {{archive.tar.gz}} to {{directory}}
```
#### Play Spotify:
```shell
betty play {{Spotify}}
```
#### Drive Betty to madness:
```shell
betty go crazy
```
{% endraw %}