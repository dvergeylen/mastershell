---
layout: default
title: "pdfjam"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfjam">
  <a href="/en/common/pdfjam.html">pdfjam</a> <a href="#pdfjam"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shell frontend for the LaTeX pdfpages package for mingling PDFs.
> More information: <https://github.com/rrthomas/pdfjam>.

#### Merge two (or more) PDFs:
```shell
pdfjam {{path/to/file1.pdf}} {{path/to/file2.pdf}} --outfile {{path/to/output_file.pdf}}
```
#### Merge the first page of each file together:
```shell
pdfjam {{files...}} 1 --outfile {{path/to/output_file.pdf}}
```
#### Merge subranges from two PDFs:
```shell
pdfjam {{path/to/file1.pdf 3-5,1}} {{path/to/file2.pdf 4-6}} --outfile {{path/to/output_file.pdf}}
```
#### Sign an A4 page (adjust delta to height for other formats) with a scanned signature by overlaying them:
```shell
pdfjam {{path/to/file.pdf}} {{path/to/signature}} --fitpaper true --outfile {{path/to/signed.pdf}} --nup "{{1x2}}" --delta "{{0 -842pt}}"
```
#### Arrange the pages from the input file into a fancy 2x2 grid:
```shell
pdfjam {{path/to/file.pdf}} --nup {{2x2}} --suffix {{4up}} --preamble '{{\usepackage{fancyhdr} \pagestyle{fancy}}}'
```
#### Reverse the order of pages within each given file and concatenate them:
```shell
pdfjam {{files...}} {{last-1}} --suffix {{reversed}}
```
{% endraw %}