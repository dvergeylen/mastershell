---
layout: default
title: "man"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="man">
  <a href="/en/common/man.html">man</a> <a href="#man"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Format and display manual pages.
> More information: <https://www.man7.org/linux/man-pages/man1/man.1.html>.

#### Display the man page for a command:
```shell
man {{command}}
```
#### Display the man page for a command from section 7:
```shell
man {{command}}.{{7}}
```
#### Display the path searched for manpages:
```shell
man --path
```
#### Display the location of a manpage rather than the manpage itself:
```shell
man -w {{command}}
```
#### Display the man page using a specific locale:
```shell
man {{command}} --locale={{locale}}
```
#### Search for manpages containing a search string:
```shell
man -k "{{search_string}}"
```
{% endraw %}