---
layout: default
title: "tee"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tee">
  <a href="/en/common/tee.html">tee</a> <a href="#tee"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read from standard input and write to standard output and files (or commands).
> More information: <https://www.gnu.org/software/coreutils/tee>.

#### Copy standard input to each FILE, and also to standard output:
```shell
echo "example" | tee {{FILE}}
```
#### Append to the given FILEs, do not overwrite:
```shell
echo "example" | tee -a {{FILE}}
```
#### Print standard input to the terminal, and also pipe it into another program for further processing:
```shell
echo "example" | tee {{/dev/tty}} | {{xargs printf "[%s]"}}
```
#### Create a directory called "example", count the number of characters in "example" and write "example" to the terminal:
```shell
echo "example" | tee >(xargs mkdir) >(wc -c)
```
{% endraw %}