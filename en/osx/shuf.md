---
layout: default
title: "shuf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shuf">
  <a href="/en/osx/shuf.html">shuf</a> <a href="#shuf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate random permutations.

#### Randomize the order of lines in a file and output the result:
```shell
shuf {{filename}}
```
#### Only output the first 5 entries of the result:
```shell
shuf -n {{5}} {{filename}}
```
#### Write output to another file:
```shell
shuf {{filename}} -o {{output_filename}}
```
#### Generate random numbers in range 1-10:
```shell
shuf -i {{1-10}}
```
{% endraw %}