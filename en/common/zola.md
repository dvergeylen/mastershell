---
layout: default
title: "zola"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zola">
  <a href="/en/common/zola.html">zola</a> <a href="#zola"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A static site generator in a single binary with everything built-in.
> More information: <https://www.getzola.org/documentation/getting-started/cli-usage/>.

#### Create the directory structure used by Zola at the given directory:
```shell
zola init {{my_site}}
```
#### Build the whole site in the `public` directory after deleting it:
```shell
zola build
```
#### Build the whole site into a different directory:
```shell
zola build --output-dir {{path/to/output_directory/}}
```
#### Build and serve the site using a local server (default is `127.0.0.1:1111`):
```shell
zola serve
```
#### Build all pages just like the build command would, but without writing any of the results to disk:
```shell
zola check
```
{% endraw %}