---
layout: default
title: "shuf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shuf">
  <a href="/en/common/shuf.html">shuf</a> <a href="#shuf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate random permutations.
> More information: <https://www.gnu.org/software/coreutils/shuf>.

#### Randomize the order of lines in a file and output the result:
```shell
shuf {{filename}}
```
#### Only output the first 5 entries of the result:
```shell
shuf --head-count={{5}} {{filename}}
```
#### Write the output to another file:
```shell
shuf {{filename}} --output={{output_filename}}
```
#### Generate 3 random numbers in the range 1-10 (inclusive):
```shell
shuf --head-count={{3}} --input-range={{1-10}} --repeat
```
{% endraw %}