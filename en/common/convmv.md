---
layout: default
title: "convmv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="convmv">
  <a href="/en/common/convmv.html">convmv</a> <a href="#convmv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert filenames (NOT file content) from one encoding to another.
> More information: <https://www.j3e.de/linux/convmv/man/>.

#### Test filename encoding conversion (don't actually change the filename):
```shell
convmv -f {{from_encoding}} -t {{to_encoding}} {{input_file}}
```
#### Convert filename encoding and rename the file to the new encoding:
```shell
convmv -f {{from_encoding}} -t {{to_encoding}} --notest {{input_file}}
```
{% endraw %}