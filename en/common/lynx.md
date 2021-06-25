---
layout: default
title: "lynx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lynx">
  <a href="/en/common/lynx.html">lynx</a> <a href="#lynx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line web browser.
> More information: <https://lynx.browser.org>.

#### Visit a website:
```shell
lynx {{example.com}}
```
#### Apply restrictions for anonymous account:
```shell
lynx -anonymous {{example.com}}
```
#### Turn on mouse support, if available:
```shell
lynx -use_mouse {{example.com}}
```
#### Force color mode on, if available:
```shell
lynx -color {{example.com}}
```
#### Open a link, using a specific file to read and write cookies:
```shell
lynx -cookie_file={{path/to/file}} {{example.com}}
```
#### Navigate forwards and backwards through the links on a page:
```shell
Up arrow key, Down arrow key
```
#### Go back to the previously displayed page:
```shell
Left arrow key or u
```
#### Exit:
```shell
q then y
```
{% endraw %}