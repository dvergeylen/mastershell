---
layout: default
title: "w3m"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="w3m">
  <a href="/en/common/w3m.html">w3m</a> <a href="#w3m"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A text-based web browser.
> Supports SSL and mouse input, even over SSH.
> More information: <http://w3m.sourceforge.net>.

#### Open a URL:
```shell
w3m {{http://example.com}}
```
#### Open a URL in monochrome mode:
```shell
w3m {{http://example.com}} -M
```
#### Open a URL without mouse support:
```shell
w3m {{http://example.com}} --no-mouse
```
#### Open a new browser tab:
```shell
Shift + T
```
#### Display your browser history:
```shell
Ctrl + H
```
#### Quit w3m:
```shell
'q' then 'y'
```
{% endraw %}