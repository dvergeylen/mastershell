---
layout: default
title: "esbuild"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="esbuild">
  <a href="/en/common/esbuild.html">esbuild</a> <a href="#esbuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> JavaScript bundler and minifier built for speed.
> More information: <https://esbuild.github.io/>.

#### Bundle a JavaScript application and print to stdout:
```shell
esbuild --bundle {{path/to/file.js}}
```
#### Bundle a JSX application from stdin:
```shell
esbuild --bundle --outfile={{path/to/out.js}} < {{path/to/file.jsx}}
```
#### Bundle and minify a JSX application with source maps in `production` mode:
```shell
esbuild --bundle --define:{{process.env.NODE_ENV=\"production\"}} --minify --sourcemap {{path/to/file.js}}
```
#### Bundle a JSX application for a comma-separated list of browsers:
```shell
esbuild --bundle --minify --sourcemap --target={{chrome58,firefox57,safari11,edge16}} {{path/to/file.jsx}}
```
#### Bundle a JavaScript application for a specific node version:
```shell
esbuild --bundle --platform={{node}} --target={{node12}} {{path/to/file.js}}
```
#### Bundle a JavaScript application enabling JSX syntax in `.js` files:
```shell
esbuild --bundle app.js --loader:{{.js=jsx}} {{path/to/file.js}}
```
#### Bundle and serve a JavaScript application on an HTTP server:
```shell
esbuild --bundle --serve={{port}} --outfile={{index.js}} {{path/to/file.js}}
```
#### Bundle a list of files to an output directory:
```shell
esbuild --bundle --outdir={{path/to/output_directory}} {{path/to/file1}} {{path/to/file2}}
```
{% endraw %}