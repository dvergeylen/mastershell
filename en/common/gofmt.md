---
layout: default
title: "gofmt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gofmt">
  <a href="/en/common/gofmt.html">gofmt</a> <a href="#gofmt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for formatting Go source code.
> More information: <https://golang.org/cmd/gofmt/>.

#### Format a file and display the result to the console:
```shell
gofmt {{source.go}}
```
#### Format a file, overwriting the original file in-place:
```shell
gofmt -w {{source.go}}
```
#### Format a file, and then simplify the code, overwriting the original file:
```shell
gofmt -s -w {{source.go}}
```
#### Print all (including spurious) errors:
```shell
gofmt -e {{source.go}}
```
{% endraw %}