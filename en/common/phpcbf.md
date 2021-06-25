---
layout: default
title: "phpcbf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpcbf">
  <a href="/en/common/phpcbf.html">phpcbf</a> <a href="#phpcbf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fix violations detected by phpcs.
> More information: <https://github.com/squizlabs/PHP_CodeSniffer>.

#### Fix issues in the specified directory (defaults to the PEAR standard):
```shell
phpcbf {{path/to/directory}}
```
#### Display a list of installed coding standards:
```shell
phpcbf -i
```
#### Specify a coding standard to validate against:
```shell
phpcbf {{path/to/directory}} --standard {{standard}}
```
#### Specify comma-separated file extensions to include when sniffing:
```shell
phpcbf {{path/to/directory}} --extensions {{file_extension(s)}}
```
#### A comma-separated list of files to load before processing:
```shell
phpcbf {{path/to/directory}} --bootstrap {{file(s)}}
```
#### Don't recurse into subdirectories:
```shell
phpcbf {{path/to/directory}} -l
```
{% endraw %}