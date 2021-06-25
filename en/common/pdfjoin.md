---
layout: default
title: "pdfjoin"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfjoin">
  <a href="/en/common/pdfjoin.html">pdfjoin</a> <a href="#pdfjoin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PDF merging utility based on pdfjam.
> More information: <https://github.com/rrthomas/pdfjam-extras>.

#### Merge two PDFs into one with the default suffix "joined":
```shell
pdfjoin {{path/to/file1.pdf}} {{path/to/file2.pdf}}
```
#### Merge the first page of each given file together:
```shell
pdfjoin {{path/to/file1.pdf path/to/file2.pdf ...}} {{1}} --outfile {{output_file}}
```
#### Save pages 3 to 5 followed by page 1 to a new PDF with custom suffix:
```shell
pdfjoin {{path/to/file.pdf}} {{3-5,1}} --suffix {{rearranged}}
```
#### Merge page subranges from two PDFs:
```shell
pdfjoin {/path/to/file1.pdf}} {{2-}} {{file2}} {{last-3}} --outfile {{output_file}}
```
{% endraw %}