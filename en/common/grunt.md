---
layout: default
title: "grunt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grunt">
  <a href="/en/common/grunt.html">grunt</a> <a href="#grunt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A JavaScript task runner for automating processes.
> More information: <https://github.com/gruntjs/grunt-cli>.

#### Run the default task process:
```shell
grunt
```
#### Run one or more specific space-separated task(s):
```shell
grunt {{task_name}}
```
#### Specify an alternative configuration file:
```shell
grunt --gruntfile {{path/to/file}}
```
#### Specify an alternative base path for relative files:
```shell
grunt --base {{path/to/directory}}
```
#### Specify an additional directory to scan for tasks in:
```shell
grunt --tasks {{path/to/directory}}
```
#### Perform a dry-run without writing any files:
```shell
grunt --no-write
```
#### List all available options:
```shell
grunt --help
```
{% endraw %}