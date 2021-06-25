---
layout: default
title: "pygmentize"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pygmentize">
  <a href="/en/common/pygmentize.html">pygmentize</a> <a href="#pygmentize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python-based syntax highlighter.

#### Highlight file syntax and print to standard output (language is inferred from the file extension):
```shell
pygmentize {{file.py}}
```
#### Explicitly set the language for syntax highlighting:
```shell
pygmentize -l {{javascript}} {{input_file}}
```
#### List available lexers (processors for input languages):
```shell
pygmentize -L lexers
```
#### Save output to a file in HTML format:
```shell
pygmentize -f html -o {{output_file.html}} {{input_file.py}}
```
#### List available output formats:
```shell
pygmentize -L formatters
```
#### Output an HTML file, with additional formatter options (full page, with line numbers):
```shell
pygmentize -f html -O "full,linenos=True" -o {{output_file.html}} {{input_file}}
```
{% endraw %}