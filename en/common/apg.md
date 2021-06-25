---
layout: default
title: "apg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apg">
  <a href="/en/common/apg.html">apg</a> <a href="#apg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates arbitrarily complex random passwords.
> More information: <https://manned.org/apg>.

#### Create random passwords (default password length is 8):
```shell
apg
```
#### Create a password with at least 1 symbol (S), 1 number (N), 1 uppercase (C), 1 lowercase (L):
```shell
apg -M SNCL
```
#### Create a password with 16 characters:
```shell
apg -m {{16}}
```
#### Create a password with maximum length of 16:
```shell
apg -x {{16}}
```
#### Create a password that doesn't appear in a dictionary (the dictionary file has to be provided):
```shell
apg -r {{dictionary_file}}
```
{% endraw %}