---
layout: default
title: "pdfseparate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfseparate">
  <a href="/en/common/pdfseparate.html">pdfseparate</a> <a href="#pdfseparate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Portable Document Format (PDF) file page extractor.
> More information: <https://manpages.debian.org/unstable/poppler-utils/pdfseparate.1.en.html>.

#### Extract pages from PDF file and make a separate PDF file for each page:
```shell
pdfseparate {{path/to/source_filename.pdf}} {{path/to/destination_filename-%d.pdf}}
```
#### Specify the first/start page for extraction:
```shell
pdfseparate -f {{3}} {{path/to/source_filename.pdf}} {{path/to/destination_filename-%d.pdf}}
```
#### Specify the last page for extraction:
```shell
pdfseparate -l {{10}} {{path/to/source_filename.pdf}} {{path/to/destination_filename-%d.pdf}}
```
{% endraw %}