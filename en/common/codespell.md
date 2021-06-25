---
layout: default
title: "codespell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="codespell">
  <a href="/en/common/codespell.html">codespell</a> <a href="#codespell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Spellchecker for source code.
> More information: <https://github.com/codespell-project/codespell>.

#### Check for typos in all text files in the current directory, recursively:
```shell
codespell
```
#### Correct all typos found in-place:
```shell
codespell --write-changes
```
#### Skip files with names that match the specified pattern (accepts a comma-separated list of patterns using wildcards):
```shell
codespell --skip "{{pattern}}"
```
#### Use a custom dictionary file when checking (`--dictionary` can be used multiple times):
```shell
codespell --dictionary {{path/to/file.txt}}
```
#### Do not check words that are listed in the specified file:
```shell
codespell --ignore-words {{path/to/file.txt}}
```
#### Do not check the specified words:
```shell
codespell --ignore-words-list {{words,to,ignore}}
```
#### Print 3 lines of context around, before or after each match:
```shell
codespell --{{context|before-context|after-context}} {{3}}
```
#### Check file names for typos, in addition to file contents:
```shell
codespell --check-filenames
```
{% endraw %}