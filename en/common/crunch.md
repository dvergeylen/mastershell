---
layout: default
title: "crunch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="crunch">
  <a href="/en/common/crunch.html">crunch</a> <a href="#crunch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wordlist generator.
> More information: <https://sourceforge.net/projects/crunch-wordlist/>.

#### Output a list of words of length 1 to 3 with only lowercase characters:
```shell
crunch {{1}} {{3}}
```
#### Output a list of hexadecimal words of length 8:
```shell
crunch {{8}} {{8}} {{0123456789abcdef}}
```
#### Output a list of all permutations of abc (lengths are not processed):
```shell
crunch {{1}} {{1}} -p {{abc}}
```
#### Output a list of all permutations of the given strings (lengths are not processed):
```shell
crunch {{1}} {{1}} -p {{abc}} {{def}} {{ghi}}
```
#### Output a list of words generated according to the given pattern and a maximum number of duplicate letters:
```shell
crunch {{5}} {{5}} {{abcde123}} -t {{@@@12}} -d 2@
```
#### Write a list of words in chunk files of a given size, starting with the given string:
```shell
crunch {{3}} {{5}} -o {{START}} -b {{10kb}} -s {{abc}}
```
#### Write a list of words stopping with the given string and inverting the wordlist:
```shell
crunch {{1}} {{5}} -o {{START}} -e {{abcde}} -i
```
#### Write a list of words in compressed chunk files with a specified number of words:
```shell
crunch {{1}} {{5}} -o {{START}} -c {{1000}} -z {{gzip|bzip2|lzma|7z}}
```
{% endraw %}