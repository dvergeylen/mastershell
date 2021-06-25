---
layout: default
title: "multitail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="multitail">
  <a href="/en/common/multitail.html">multitail</a> <a href="#multitail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extension of tail.
> More information: <https://www.vanheusden.com/multitail/examples.php>.

#### Tail all files matching a pattern in a single stream:
```shell
multitail -Q 1 '{{pattern}}'
```
#### Tail all files in a directory in a single stream:
```shell
multitail -Q 1 '{{directory}}/*'
```
#### Automatically add new files to a window:
```shell
multitail -Q {{pattern}}
```
#### Show 5 logfiles while merging 2 and put them in 2 columns with only one in the left column:
```shell
multitail -s 2 -sn 1,3 {{mergefile}} -I {{file1}} {{file2}} {{file3}} {{file4}}
```
{% endraw %}