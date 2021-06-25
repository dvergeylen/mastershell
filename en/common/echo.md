---
layout: default
title: "echo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="echo">
  <a href="/en/common/echo.html">echo</a> <a href="#echo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print given arguments.
> More information: <https://www.gnu.org/software/coreutils/echo>.

#### Print a text message. Note: quotes are optional:
```shell
echo "{{Hello World}}"
```
#### Print a message with environment variables:
```shell
echo "{{My path is $PATH}}"
```
#### Print a message without the trailing newline:
```shell
echo -n "{{Hello World}}"
```
#### Append a message to the file:
```shell
echo "{{Hello World}}" >> {{file.txt}}
```
#### Enable interpretation of backslash escapes (special characters):
```shell
echo -e "{{Column 1\tColumn 2}}"
```
{% endraw %}