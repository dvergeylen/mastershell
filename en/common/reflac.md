---
layout: default
title: "reflac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reflac">
  <a href="/en/common/reflac.html">reflac</a> <a href="#reflac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recompress FLAC files in-place while preserving metadata.
> More information: <https://github.com/chungy/reflac>.

#### Recompress a directory of FLAC files:
```shell
reflac {{path/to/directory}}
```
#### Enable maximum compression (very slow):
```shell
reflac --best {{path/to/directory}}
```
#### Display filenames as they are processed:
```shell
reflac --verbose {{path/to/directory}}
```
#### Recurse into subdirectories:
```shell
reflac --recursive {{path/to/directory}}
```
#### Preserve file modification times:
```shell
reflac --preserve {{path/to/directory}}
```
{% endraw %}