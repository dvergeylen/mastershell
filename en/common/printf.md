---
layout: default
title: "printf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="printf">
  <a href="/en/common/printf.html">printf</a> <a href="#printf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Format and print text.
> More information: <https://www.gnu.org/software/coreutils/printf>.

#### Print a text message:
```shell
printf "{{%s\n}}" "{{Hello world}}"
```
#### Print an integer in bold blue:
```shell
printf "{{\e[1;34m%.3d\e[0m\n}}" {{42}}
```
#### Print a float number with the Unicode Euro sign:
```shell
printf "{{\u20AC %.2f\n}}" {{123.4}}
```
#### Print a text message composed with environment variables:
```shell
printf "{{var1: %s\tvar2: %s\n}}" "{{$VAR1}}" "{{$VAR2}}"
```
#### Store a formatted message in a variable (does not work on zsh):
```shell
printf -v {{myvar}} {{"This is %s = %d\n" "a year" 2016}}
```
{% endraw %}