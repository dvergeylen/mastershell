---
layout: default
title: "phpcpd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpcpd">
  <a href="/en/common/phpcpd.html">phpcpd</a> <a href="#phpcpd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A copy and paste detector for PHP code.
> More information: <https://github.com/sebastianbergmann/phpcpd>.

#### Analyse duplicated code for a specific file or directory:
```shell
phpcpd {{path/to/file_or_directory}}
```
#### Analyse using fuzzy matching for variable names:
```shell
phpcpd --fuzzy {{path/to/file_or_directory}}
```
#### Specify a minimum number of identical lines (defaults to 5):
```shell
phpcpd --min-lines {{number_of_lines}} {{path/to/file_or_directory}}
```
#### Specify a minimum number of identical tokens (defaults to 70):
```shell
phpcpd --min-tokens {{number_of_tokens}} {{path/to/file_or_directory}}
```
#### Exclude a directory from analysis (must be relative to the source):
```shell
phpcpd --exclude {{path/to/excluded_directory}} {{path/to/file_or_directory}}
```
#### Output the results to a PHP-CPD XML file:
```shell
phpcpd --log-pmd {{path/to/log_file}} {{path/to/file_or_directory}}
```
{% endraw %}