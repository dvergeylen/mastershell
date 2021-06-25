---
layout: default
title: "web-ext"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="web-ext">
  <a href="/en/common/web-ext.html">web-ext</a> <a href="#web-ext"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for managing web extension development.
> More information: <https://www.npmjs.com/package/web-ext>.

#### Run the web extension in the current directory in Firefox:
```shell
web-ext run
```
#### Run a web extension from a specific directory in Firefox:
```shell
web-ext run --source-dir {{path/to/directory}}
```
#### Display verbose execution output:
```shell
web-ext run --verbose
```
#### Run a web extension in Firefox Android:
```shell
web-ext run --target firefox-android
```
#### Lint the manifest and source files for errors:
```shell
web-ext lint
```
#### Build and package the extension:
```shell
web-ext build
```
#### Display verbose build output:
```shell
web-ext build --verbose
```
#### Sign a package for self-hosting:
```shell
web-ext sign --api-key {{api_key}} --api-secret {{api_secret}}
```
{% endraw %}