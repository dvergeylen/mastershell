---
layout: default
title: "read"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="read">
  <a href="/en/common/read.html">read</a> <a href="#read"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> BASH builtin for retrieving data from standard input.

#### Store data that you type from the keyboard:
```shell
read {{variable}}
```
#### Store each of the next lines you enter as values of an array:
```shell
read -a {{array}}
```
#### Specify the number of maximum characters to be read:
```shell
read -n {{character_count}} {{variable}}
```
#### Use a specific character as a delimiter instead of a new line:
```shell
read -d {{new_delimiter}} {{variable}}
```
#### Do not let backslash (\) act as an escape character:
```shell
read -r {{variable}}
```
#### Display a prompt before the input:
```shell
read -p "{{Enter your input here: }}" {{variable}}
```
#### Do not echo typed characters (silent mode):
```shell
read -s {{variable}}
```
#### Read stdin and perform an action on every line:
```shell
while read line; do echo "$line"; done
```
{% endraw %}