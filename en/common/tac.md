---
layout: default
title: "tac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tac">
  <a href="/en/common/tac.html">tac</a> <a href="#tac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print and concatenate files in reverse (last line first).
> More information: <https://www.gnu.org/software/coreutils/tac>.

#### Print the contents of *file1* reversed to the standard output:
```shell
tac {{file1}}
```
#### Print the contents of the standard input reversed to the standard output:
```shell
{{command}} | tac
```
#### Concatenate several files reversed into the target file:
```shell
tac {{file1}} {{file2}} > {{target_file}}
```
{% endraw %}