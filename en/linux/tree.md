---
layout: default
title: "tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tree">
  <a href="/en/linux/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show the contents of the current directory as a tree.
> More information: <http://mama.indstate.edu/users/ice/tree/>.

#### Print files and directories up to 'num' levels of depth (where 1 means the current directory):
```shell
tree -L {{num}}
```
#### Print directories only:
```shell
tree -d
```
#### Print hidden files too with colorization on:
```shell
tree -a -C
```
#### Print the tree without indentation lines, showing the full path instead (use `-N` to not escape non-printable characters):
```shell
tree -i -f
```
#### Print the size of each file and the cumulative size of each directory, in human-readable format:
```shell
tree -s -h --du
```
#### Print files within the tree hierarchy, using a wildcard (glob) pattern, and pruning out directories that don't contain matching files:
```shell
tree -P '{{*.txt}}' --prune
```
#### Print directories within the tree hierarchy, using the wildcard (glob) pattern, and pruning out directories that aren't ancestors of the wanted one:
```shell
tree -P {{directory_name}} --matchdirs --prune
```
#### Print the tree ignoring the given directories:
```shell
tree -I '{{directory_name1|directory_name2}}'
```
{% endraw %}