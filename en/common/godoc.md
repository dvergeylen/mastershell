---
layout: default
title: "godoc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="godoc">
  <a href="/en/common/godoc.html">godoc</a> <a href="#godoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show documentation for go packages.
> More information: <https://godoc.org/>.

#### Display help for package "fmt":
```shell
godoc {{fmt}}
```
#### Display help for the function "Printf" of "fmt" package:
```shell
godoc {{fmt}} {{Printf}}
```
#### Serve documentation as a web server on port 6060:
```shell
godoc -http=:{{6060}}
```
#### Create an index file:
```shell
godoc -write_index -index_files={{path/to/file}}
```
#### Use the given index file to search the docs:
```shell
godoc -http=:{{6060}} -index -index_files={{path/to/file}}
```
{% endraw %}