---
layout: default
title: "xcursorgen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xcursorgen">
  <a href="/en/linux/xcursorgen.html">xcursorgen</a> <a href="#xcursorgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create an X cursor file from a collection of PNG images.
> If `--prefix` is omitted, the image files must be located in the current working directory.
> More information: <https://manned.org/xcursorgen.1>.

#### Create an X cursor file using a config file:
```shell
xcursorgen {{path/to/config.cursor}} {{path/to/output_file}}
```
#### Create an X cursor file using a config file and specify the path to the image files:
```shell
xcursorgen --prefix {{path/to/image_directory/}} {{path/to/config.cursor}} {{path/to/output_file}}
```
#### Create an X cursor file using a config file and write the output to stdout:
```shell
xcursorgen {{path/to/config.cursor}}
```
{% endraw %}