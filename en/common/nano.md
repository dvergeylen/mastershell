---
layout: default
title: "nano"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nano">
  <a href="/en/common/nano.html">nano</a> <a href="#nano"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple, easy to use command-line text editor. An enhanced, free Pico clone.
> More information: <https://nano-editor.org>.

#### Open a specific file:
```shell
nano {{path/to/file}}
```
#### Open a file positioning the cursor at the specified line and column:
```shell
nano +{{line}},{{column}} {{path/to/file}}
```
#### Enable smooth scrolling:
```shell
nano -S {{filename}}
```
#### Indent new lines to the previous lines' indentation:
```shell
nano -i {{filename}}
```
#### Before modification, backup separately as `{{current_file_name}}~`:
```shell
nano -B {{filename}}
```
{% endraw %}