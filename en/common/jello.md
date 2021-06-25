---
layout: default
title: "jello"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jello">
  <a href="/en/common/jello.html">jello</a> <a href="#jello"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line JSON processor using Python syntax.
> More information: <https://github.com/kellyjonbrazil/jello>.

#### Pretty-print JSON or JSON-Lines data from stdin to stdout:
```shell
cat {{file.json}} | jello
```
#### Output a schema of JSON or JSON Lines data from stdin to stdout (useful for grep):
```shell
cat {{file.json}} | jello -s
```
#### Output all elements from arrays (or all the values from objects) in JSON or JSON-Lines data from stdin to stdout:
```shell
cat {{file.json}} | jello -l
```
#### Output the first element in JSON or JSON-Lines data from stdin to stdout:
```shell
cat {{file.json}} | jello _[0]
```
#### Output the value of a given key of each element in JSON or JSON-Lines data from stdin to stdout:
```shell
cat {{file.json}} | jello '[i.{{key_name}} for i in _]'
```
#### Output the value of multiple keys as a new JSON object (assuming the input JSON has the keys `key_name` and `other_key_name`):
```shell
cat {{file.json}} | jello '{"{{my_new_key}}": _.{{key_name}}, "{{my_other_key}}": _.{{other_key_name}}}'
```
#### Output the value of a given key to a string (and disable JSON output):
```shell
cat {{file.json}} | jello -r '"{{some text}}: " + _.{{key_name}}'
```
{% endraw %}