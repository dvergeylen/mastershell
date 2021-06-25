---
layout: default
title: "phploc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phploc">
  <a href="/en/common/phploc.html">phploc</a> <a href="#phploc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for quickly measuring the size and analyzing the structure of a PHP project.
> More information: <https://github.com/sebastianbergmann/phploc>.

#### Analyse a directory and print the result:
```shell
phploc {{path/to/directory}}
```
#### Include only specific files from a comma-separated list (globs are allowed):
```shell
phploc {{path/to/directory}} --names {{files}}
```
#### Exclude specific files from a comma-separated list (globs are allowed):
```shell
phploc {{path/to/directory}} --names-exclude {{files}}
```
#### Exclude a specific directory from analysis:
```shell
phploc {{path/to/directory}} --exclude {{path/to/exclude_directory}}
```
#### Log the results to a specific CSV file:
```shell
phploc {{path/to/directory}} --log-csv {{path/to/file}}
```
#### Log the results to a specific XML file:
```shell
phploc {{path/to/directory}} --log-xml {{path/to/file}}
```
#### Count PHPUnit test case classes and test methods:
```shell
phploc {{path/to/directory}} --count-tests
```
{% endraw %}