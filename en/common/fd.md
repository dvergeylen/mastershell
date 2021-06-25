---
layout: default
title: "fd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fd">
  <a href="/en/common/fd.html">fd</a> <a href="#fd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An alternative to `find`.
> Aims to be faster and easier to use than `find`.
> More information: <https://github.com/sharkdp/fd>.

#### Recursively find files matching the given pattern in the current directory:
```shell
fd {{pattern}}
```
#### Find files that begin with "foo":
```shell
fd {{'^foo'}}
```
#### Find files with a specific extension:
```shell
fd --extension {{txt}}
```
#### Find files in a specific directory:
```shell
fd {{pattern}} {{path/to/directory}}
```
#### Include ignored and hidden files in the search:
```shell
fd --hidden --no-ignore {{pattern}}
```
#### Execute a command on each search result returned:
```shell
fd {{pattern}} --exec {{command}}
```
{% endraw %}