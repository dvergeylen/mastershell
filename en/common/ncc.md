---
layout: default
title: "ncc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ncc">
  <a href="/en/common/ncc.html">ncc</a> <a href="#ncc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile a Node.js application into a single file.
> Supports TypeScript, binary addons and dynamic requires.
> More information: <https://github.com/vercel/ncc>.

#### Bundle a Node.js application:
```shell
ncc build {{path/to/file.js}}
```
#### Bundle and minify a Node.js application:
```shell
ncc build --minify {{path/to/file.js}}
```
#### Bundle and minify a Node.js application and generate source maps:
```shell
ncc build --source-map {{path/to/file.js}}
```
#### Automatically recompile on changes to source files:
```shell
ncc build --watch {{path/to/file.js}}
```
#### Bundle a Node.js application into a temporary directory and run it for testing:
```shell
ncc run {{path/to/file.js}}
```
#### Clean the `ncc` cache:
```shell
ncc clean cache
```
{% endraw %}