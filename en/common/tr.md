---
layout: default
title: "tr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tr">
  <a href="/en/common/tr.html">tr</a> <a href="#tr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Translate characters: run replacements based on single characters and character sets.
> More information: <https://www.gnu.org/software/coreutils/tr>.

#### Replace all occurrences of a character in a file, and print the result:
```shell
tr {{find_character}} {{replace_character}} < {{filename}}
```
#### Replace all occurrences of a character from another command's output:
```shell
echo {{text}} | tr {{find_character}} {{replace_character}}
```
#### Map each character of the first set to the corresponding character of the second set:
```shell
tr '{{abcd}}' '{{jkmn}}' < {{filename}}
```
#### Delete all occurrences of the specified set of characters from the input:
```shell
tr -d '{{input_characters}}' < {{filename}}
```
#### Compress a series of identical characters to a single character:
```shell
tr -s '{{input_characters}}' < {{filename}}
```
#### Translate the contents of a file to upper-case:
```shell
tr "[:lower:]" "[:upper:]" < {{filename}}
```
#### Strip out non-printable characters from a file:
```shell
tr -cd "[:print:]" < {{filename}}
```
{% endraw %}