---
layout: default
title: "alex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alex">
  <a href="/en/common/alex.html">alex</a> <a href="#alex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool that catches insensitive, inconsiderate writing.
> It helps you find gender favouring, polarising, race related, religion inconsiderate, or other unequal phrasing in text.
> More information: <https://github.com/get-alex/alex>.

#### Analyze text from stdin:
```shell
echo {{His network looks good}} | alex --stdin
```
#### Analyze all files in the current directory:
```shell
alex
```
#### Analyze a specific file:
```shell
alex {{textfile.md}}
```
#### Analyze all Markdown files except `example.md`:
```shell
alex *.md !{{example.md}}
```
{% endraw %}