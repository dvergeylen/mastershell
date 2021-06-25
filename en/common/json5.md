---
layout: default
title: "json5"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="json5">
  <a href="/en/common/json5.html">json5</a> <a href="#json5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for converting JSON5 files to JSON.
> More information: <https://json5.org>.

#### Convert JSON5 stdin to JSON stdout:
```shell
echo {{input}} | json5
```
#### Convert a JSON5 file to JSON and output to stdout:
```shell
json5 {{path/to/input_file.json5}}
```
#### Convert a JSON5 file to the specified JSON file:
```shell
json5 {{path/to/input_file.json5}} --out-file {{path/to/output_file.json}}
```
#### Validate a JSON5 file:
```shell
json5 {{path/to/input_file.json5}} --validate
```
#### Specify the number of spaces to indent by (or "t" for tabs):
```shell
json5 --space {{indent_amount}}
```
#### View available options:
```shell
json5 --help
```
{% endraw %}