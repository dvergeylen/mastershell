---
layout: default
title: "enscript"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="enscript">
  <a href="/en/common/enscript.html">enscript</a> <a href="#enscript"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert text files to PostScript, HTML, RTF, ANSI, and overstrikes.
> More information: <https://www.gnu.org/software/enscript>.

#### Generate a PostScript file from a text file:
```shell
enscript {{path/to/input_file}} --output={{path/to/output_file}}
```
#### Generate a file in a different language than PostScript:
```shell
enscript {{path/to/input_file}} --language={{html|rtf|...}} --output={{path/to/output_file}}
```
#### Generate a PostScript file with a landscape layout, splitting the page into columns (maximum 9):
```shell
enscript {{path/to/input_file}} --columns={{num}} --landscape --output={{path/to/output_file}}
```
#### Display available syntax highlighting languages and file formats:
```shell
enscript --help-highlight
```
#### Generate a PostScript file with syntax highlighting and color for a specified language:
```shell
enscript {{path/to/input_file}} --color=1 --highlight={{language}} --output={{path/to/output_file}}
```
{% endraw %}