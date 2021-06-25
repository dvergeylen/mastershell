---
layout: default
title: "lilypond"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lilypond">
  <a href="/en/common/lilypond.html">lilypond</a> <a href="#lilypond"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Typeset music and/or produce MIDI from file.
> More information: <https://lilypond.org>.

#### Compile a lilypond file into a PDF:
```shell
lilypond {{path/to/file}}
```
#### Compile into the specified format:
```shell
lilypond --formats={{format_dump}} {{path/to/file}}
```
#### Compile the specified file, suppressing progress updates:
```shell
lilypond -s {{path/to/file}}
```
#### Compile the specified file, and also specify the output filename:
```shell
lilypond --output={{path/to/output_file}} {{path/to/input_file}}
```
#### Show the current version of lilypond:
```shell
lilypond --version
```
{% endraw %}