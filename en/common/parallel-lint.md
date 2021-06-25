---
layout: default
title: "parallel-lint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="parallel-lint">
  <a href="/en/common/parallel-lint.html">parallel-lint</a> <a href="#parallel-lint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to check the syntax of PHP files in parallel.
> More information: <https://github.com/JakubOnderka/PHP-Parallel-Lint>.

#### Lint a specific directory:
```shell
parallel-lint {{path/to/directory}}
```
#### Lint a directory using the specified number of parallel processes:
```shell
parallel-lint -j {{processes}} {{path/to/directory}}
```
#### Lint a directory, excluding the specified directory:
```shell
parallel-lint --exclude {{path/to/excluded_directory}} {{path/to/directory}}
```
#### Lint a directory of files using a comma-separated list of extension(s):
```shell
parallel-lint -e {{php,html,phpt}} {{path/to/directory}}
```
#### Lint a directory and output the results as JSON:
```shell
parallel-lint --json {{path/to/directory}}
```
#### Lint a directory and show Git Blame results for rows containing errors:
```shell
parallel-lint --blame {{path/to/directory}}
```
{% endraw %}