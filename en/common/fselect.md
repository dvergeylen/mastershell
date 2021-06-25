---
layout: default
title: "fselect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fselect">
  <a href="/en/common/fselect.html">fselect</a> <a href="#fselect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find files with SQL-like queries.
> More information: <https://github.com/jhspetersson/fselect>.

#### Select full path and size from temporary or config files in a given directory:
```shell
fselect size, path from {{path/to/directory}} where name = {{'*.cfg'}} or name = {{'*.tmp'}}
```
#### Find square images:
```shell
fselect path from {{path/to/directory}} where width = height
```
#### Find old-school rap 320kbps MP3 files:
```shell
fselect path from {{path/to/directory}} where genre = {{Rap}} and bitrate = {{320}} and mp3_year lt {{2000}}
```
#### Select only the first 5 results and output as JSON:
```shell
fselect size, path from {{path/to/directory}} limit {{5}} into json
```
#### Use SQL aggregate functions to calculate minimum, maximum and average size of files in a directory:
```shell
fselect "{{MIN(size), MAX(size), AVG(size), SUM(size), COUNT(*)}} from {{path/to/directory}}"
```
{% endraw %}