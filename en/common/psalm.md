---
layout: default
title: "psalm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="psalm">
  <a href="/en/common/psalm.html">psalm</a> <a href="#psalm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A static analysis tool for finding errors in PHP applications.
> More information: <https://psalm.dev>.

#### Generate a Psalm configuration:
```shell
psalm --init
```
#### Analyse the current working directory:
```shell
psalm
```
#### Analyse a specific directory or file:
```shell
psalm {{path/to/file_or_directory}}
```
#### Analyse a project with a specific configuration file:
```shell
psalm --config {{path/to/psalm.xml}}
```
#### Include informational findings in the output:
```shell
psalm --show-info
```
#### Analyse a project and display statistics:
```shell
psalm --stats
```
#### Analyse a project in parallel with 4 threads:
```shell
psalm --threads {{4}}
```
{% endraw %}