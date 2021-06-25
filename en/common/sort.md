---
layout: default
title: "sort"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sort">
  <a href="/en/common/sort.html">sort</a> <a href="#sort"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sort lines of text files.
> More information: <https://www.gnu.org/software/coreutils/sort>.

#### Sort a file in ascending order:
```shell
sort {{path/to/file}}
```
#### Sort a file in descending order:
```shell
sort --reverse {{path/to/file}}
```
#### Sort a file in case-insensitive way:
```shell
sort --ignore-case {{path/to/file}}
```
#### Sort a file using numeric rather than alphabetic order:
```shell
sort --numeric-sort {{path/to/file}}
```
#### Sort `/etc/passwd` by the 3rd field of each line numerically, using ":" as a field separator:
```shell
sort --field-separator={{:}} --key={{3n}} {{/etc/passwd}}
```
#### Sort a file preserving only unique lines:
```shell
sort --unique {{path/to/file}}
```
#### Sort a file, printing the output to the specified output file (can be used to sort a file in-place):
```shell
sort --output={{path/to/file}} {{path/to/file}}
```
#### Sort numbers with exponents:
```shell
sort --general-numeric-sort {{path/to/file}}
```
{% endraw %}