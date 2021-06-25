---
layout: default
title: "dvc diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-diff">
  <a href="/en/common/dvc-diff.html">dvc diff</a> <a href="#dvc-diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show changes in DVC tracked file and directories.
> More information: <https://dvc.org/doc/command-reference/diff>.

#### Compare DVC tracked files from different Git commits, tags, and branches w.r.t the current workspace:
```shell
dvc diff {{commit_hash/tag/branch}}
```
#### Compare the changes in DVC tracked files from 1 Git commit to another:
```shell
dvc diff {{revision_b}} {{revision_a}}
```
#### Compare DVC tracked files, along with their latest hash:
```shell
dvc diff --show-hash {{commit}}
```
#### Compare DVC tracked files, displaying the output as JSON:
```shell
dvc diff --show-json --show-hash {{commit}}
```
#### Compare DVC tracked files, displaying the output as Markdown:
```shell
dvc diff --show-md --show-hash {{commit}}
```
{% endraw %}