---
layout: default
title: "monodevelop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="monodevelop">
  <a href="/en/common/monodevelop.html">monodevelop</a> <a href="#monodevelop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cross platform IDE for C#, F# and more.
> More information: <https://www.monodevelop.com/>.

#### Start MonoDevelop:
```shell
monodevelop
```
#### Open a specific file:
```shell
monodevelop {{path/to/file}}
```
#### Open a specific file with the caret at a specific position:
```shell
monodevelop {{path/to/file}};{{line_number}};{{column_number}}
```
#### Force opening a new window instead of switching to an existing one:
```shell
monodevelop --new-window
```
#### Disable redirection of stdout and stderr to a log file:
```shell
monodevelop --no-redirect
```
#### Enable performance monitoring:
```shell
monodevelop --perf-log
```
{% endraw %}