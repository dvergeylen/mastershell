---
layout: default
title: "more"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="more">
  <a href="/en/common/more.html">more</a> <a href="#more"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open a file for interactive reading, allowing scrolling and search.
> More information: <https://manned.org/more>.

#### Open a file:
```shell
more {{path/to/file}}
```
#### Open a file displaying from a specific line:
```shell
more +{{line_number}} {{path/to/file}}
```
#### Display help:
```shell
more --help
```
#### Go to the next page:
```shell
<Space>
```
#### Search for a string (press `n` to go to the next match):
```shell
/{{something}}
```
#### Exit:
```shell
q
```
#### Display help about interactive commands:
```shell
h
```
{% endraw %}