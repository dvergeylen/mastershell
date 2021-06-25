---
layout: default
title: "if"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="if">
  <a href="/en/common/if.html">if</a> <a href="#if"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple shell conditional.
> See also: `test`, `[`.

#### Execute two different commands based on a condition:
```shell
if {{command}}; then {{echo "true"}}; else {{echo "false"}}; fi
```
#### Check if a variable is defined:
```shell
if [[ -n "{{$VARIABLE}}" ]]; then {{echo "defined"}}; else {{echo "not defined"}}; fi
```
#### Check if a file exists:
```shell
if [[ -f "{{path/to/file}}" ]]; then {{echo "true"}}; else {{echo "false"}}; fi
```
#### Check if a directory exists:
```shell
if [[ -d "{{path/to/directory}}" ]]; then {{echo "true"}}; else {{echo "false"}}; fi
```
#### Check if a file or directory exists:
```shell
if [[ -e "{{path/to/file_or_directory}}" ]]; then {{echo "true"}}; else {{echo "false"}}; fi
```
#### List all possible conditions (`test` is an alias to `[`; both are commonly used with `if`):
```shell
man [
```
{% endraw %}