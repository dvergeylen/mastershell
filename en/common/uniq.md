---
layout: default
title: "uniq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uniq">
  <a href="/en/common/uniq.html">uniq</a> <a href="#uniq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Output the unique lines from the given input or file.
> Since it does not detect repeated lines unless they are adjacent, we need to sort them first.
> More information: <https://www.gnu.org/software/coreutils/uniq>.

#### Display each line once:
```shell
sort {{file}} | uniq
```
#### Display only unique lines:
```shell
sort {{file}} | uniq -u
```
#### Display only duplicate lines:
```shell
sort {{file}} | uniq -d
```
#### Display number of occurrences of each line along with that line:
```shell
sort {{file}} | uniq -c
```
#### Display number of occurrences of each line, sorted by the most frequent:
```shell
sort {{file}} | uniq -c | sort -nr
```
{% endraw %}