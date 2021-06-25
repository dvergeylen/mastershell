---
layout: default
title: "cloc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cloc">
  <a href="/en/common/cloc.html">cloc</a> <a href="#cloc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Count, and compute differences of, lines of source code and comments.
> More information: <https://github.com/AlDanial/cloc>.

#### Count all the lines of code in a directory:
```shell
cloc {{path/to/directory}}
```
#### Count all the lines of code in a directory, displaying a progress bar during the counting process:
```shell
cloc --progress=1 {{path/to/directory}}
```
#### Compare 2 directory structures and count the differences between them:
```shell
cloc --diff {{path/to/directory/one}} {{path/to/directory/two}}
```
#### Ignore files that are ignored by VCS, such as files specified in `.gitignore`:
```shell
cloc --vcs git {{path/to/directory}}
```
#### Count all the lines of code in a directory, displaying the results for each file instead of each language:
```shell
cloc --by-file {{path/to/directory}}
```
{% endraw %}