---
layout: default
title: "fcrackzip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fcrackzip">
  <a href="/en/linux/fcrackzip.html">fcrackzip</a> <a href="#fcrackzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ZIP archive password cracking utility.

#### Brute-force a password with a length of 4 to 8 characters, and contains only alphanumeric characters (order matters):
```shell
fcrackzip --brute-force --length 4-8 --charset aA1 {{archive}}
```
#### Brute-force a password in verbose mode with a length of 3 characters that only contains lowercase characters, `$` and `%`:
```shell
fcrackzip -v --brute-force --length 3 --charset a:$% {{archive}}
```
#### Brute-force a password that contains only lowercase and special characters:
```shell
fcrackzip --brute-force --length 4 --charset a! {{archive}}
```
#### Brute-force a password containing only digits, starting from the password `12345`:
```shell
fcrackzip --brute-force --length 5 --charset 1 --init-password 12345 {{archive}}
```
#### Crack a password using a wordlist:
```shell
fcrackzip --use-unzip --dictionary --init-password {{wordlist}} {{archive}}
```
#### Benchmark cracking performance:
```shell
fcrackzip --benchmark
```
{% endraw %}