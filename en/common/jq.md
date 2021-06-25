---
layout: default
title: "jq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jq">
  <a href="/en/common/jq.html">jq</a> <a href="#jq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line JSON processor that uses a domain-specific language.
> More information: <https://stedolan.github.io/jq>.

#### Output a JSON file, in pretty-print format:
```shell
jq . {{file.json}}
```
#### Output all elements from arrays (or all the values from objects) in a JSON file:
```shell
jq '.[]' {{file.json}}
```
#### Read JSON objects from a file into an array, and output it (inverse of `jq .[]`):
```shell
jq --slurp . {{file.json}}
```
#### Output the first element in a JSON file:
```shell
jq '.[0]' {{file.json}}
```
#### Output the value of a given key of each element in a JSON text from stdin:
```shell
cat {{file.json}} | jq 'map(.{{key_name}})'
```
#### Output the value of multiple keys as a new JSON object (assuming the input JSON has the keys `key_name` and `other_key_name`):
```shell
cat {{file.json}} | jq '{{{my_new_key}}: .{{key_name}}, {{my_other_key}}: .{{other_key_name}}}'
```
#### Combine multiple filters:
```shell
cat {{file.json}} | jq 'unique | sort | reverse'
```
#### Output the value of a given key to a string (and disable JSON output):
```shell
cat {{file.json}} | jq --raw-output '"some text: \(.{{key_name}})"'
```
{% endraw %}