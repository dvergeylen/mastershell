---
layout: default
title: "lpr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lpr">
  <a href="/en/common/lpr.html">lpr</a> <a href="#lpr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CUPS tool for printing files.
> See also `lpstat` and `lpadmin` for listing and configuring printers.
> More information: <http://www.CUPS.org>.

#### Print a file to the default printer:
```shell
lpr {{path/to/file}}
```
#### Print 2 copies:
```shell
lpr -# {{2}} {{path/to/file}}
```
#### Print to a named printer:
```shell
lpr -P {{printer}} {{path/to/file}}
```
#### Print either a single page (e.g. 2) or a range of pages (e.g. 2–16):
```shell
lpr -o page-ranges={{2|2-16}} {{path/to/file}}
```
#### Print double sided either in portrait (long) or in landscape (short):
```shell
lpr -o sides={{two_sided_long_edge|two_sided_short_edge}} {{path/to/file}}
```
#### Set page size (more options may be available depending on setup):
```shell
lpr -o media={{a4|letter|legal}} {{path/to/file}}
```
#### Print multiple pages per sheet:
```shell
lpr -o number-up={{2|4|6|9|16}} {{path/to/file}}
```
{% endraw %}