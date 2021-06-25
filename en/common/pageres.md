---
layout: default
title: "pageres"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pageres">
  <a href="/en/common/pageres.html">pageres</a> <a href="#pageres"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Capture screenshots of websites in various resolutions.
> More information: <https://github.com/sindresorhus/pageres-cli>.

#### Take multiple screenshots of multiple URLs at different resolutions:
```shell
pageres {{https://example.com/}} {{https://example2.com/}} {{1366x768}} {{1600x900}}
```
#### Provide specific options for a URL, overriding global options:
```shell
pageres [{{https://example.com/}} {{1366x768}} --no-crop] [{{https://example2.com/}} {{1024x768}}] --crop
```
#### Provide a custom filename template:
```shell
pageres {{https://example.com/}} {{1024x768}} --filename={{'<%= date %> - <%= url %>'}}
```
#### Capture a specific element on a page:
```shell
pageres {{https://example.com/}} {{1366x768}} --selector='{{.page-header}}'
```
#### Hide a specific element:
```shell
pageres {{https://example.com/}} {{1366x768}} --hide='{{.page-header}}'
```
#### Capture a screenshot of a local file:
```shell
pageres {{local_file_path.html}} {{1366x768}}
```
{% endraw %}