---
layout: default
title: "mcookie"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mcookie">
  <a href="/en/linux/mcookie.html">mcookie</a> <a href="#mcookie"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generates random 128 bit hexadecimal numbers.

#### Generate a random number:
```shell
mcookie
```
#### Generate a random number, using the contents of a file as a seed for the randomness:
```shell
mcookie --file {{path/to/file}}
```
#### Generate a random number, using a specific number of bytes from a file as a seed for the randomness:
```shell
mcookie --file {{path/to/file}} --max-size {{number_of_bytes}}
```
#### Print the details of the randomness used, such as the origin and seed for each source:
```shell
mcookie --verbose
```
{% endraw %}