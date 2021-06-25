---
layout: default
title: "dillo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dillo">
  <a href="/en/common/dillo.html">dillo</a> <a href="#dillo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A lightweight web browser intended for slow computers.
> More information: <https://www.dillo.org/>.

#### Launch Dillo:
```shell
dillo
```
#### Launch Dillo with a specific window size and screen location:
```shell
dillo --geometry {{width}}x{{height}}+{{x_position}}+{{y_position}}
```
#### Launch Dillo and open a specific URL:
```shell
dillo {{duckduckgo.com}}
```
#### Launch Dillo and open a file or directory:
```shell
dillo {{path/to/file_or_directory}}
```
#### Launch Dillo in full-screen mode:
```shell
dillo --fullwindow
```
#### Display version:
```shell
dillo --version
```
#### Display help:
```shell
dillo --help
```
{% endraw %}