---
layout: default
title: "git fame"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-fame">
  <a href="/en/common/git-fame.html">git fame</a> <a href="#git-fame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pretty-print Git repository contributions.
> More information: <https://github.com/casperdcl/git-fame>.

#### Calculate contributions for the current Git repository:
```shell
git fame
```
#### Exclude files/directories that match the specified regular expression:
```shell
git fame --excl "{{regular_expression}}"
```
#### Calculate contributions made after the specified date:
```shell
git fame --since "{{3 weeks ago|2021-05-13}}"
```
#### Display contributions in the specified format:
```shell
git fame --format {{pipe|yaml|json|csv|tsv}}
```
#### Display contributions per file extension:
```shell
git fame --bytype
```
#### Ignore whitespace changes:
```shell
git fame --ignore-whitespace
```
#### Detect inter-file line moves and copies:
```shell
git fame -C
```
#### Detect intra-file line moves and copies:
```shell
git fame -M
```
{% endraw %}