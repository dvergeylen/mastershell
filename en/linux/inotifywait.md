---
layout: default
title: "inotifywait"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="inotifywait">
  <a href="/en/linux/inotifywait.html">inotifywait</a> <a href="#inotifywait"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Waits for changes to one or more files.

#### Run a command when a file changes:
```shell
while inotifywait {{path/to/file}}; do {{command}}; done
```
#### Be quiet about watching for changes:
```shell
while inotifywait --quiet {{path/to/file}}; do {{command}}; done
```
#### Watch a directory recursively for changes:
```shell
while inotifywait --recursive {{path/to/directory}}; do {{command}}; done
```
#### Exclude files matching a regular expression:
```shell
while inotifywait --recursive {{path/to/directory}} --exlude '{{regular_expression}}'; do {{command}}; done
```
#### Wait at most 30 seconds:
```shell
while inotifywait --timeout {{30}} {{path/to/file}}; do {{command}}; done
```
#### Only watch for file modification events:
```shell
while inotifywait --event {{modify}} {{path/to/file}}; do {{command}}; done
```
{% endraw %}