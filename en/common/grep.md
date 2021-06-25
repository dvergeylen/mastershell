---
layout: default
title: "grep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grep">
  <a href="/en/common/grep.html">grep</a> <a href="#grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find patterns in files using regular expressions.
> More information: <https://www.gnu.org/software/grep/manual/grep.html>.

#### Search for a pattern within a file:
```shell
grep "{{search_pattern}}" {{path/to/file}}
```
#### Search for an exact string (disables regular expressions):
```shell
grep --fixed-strings "{{exact_string}}" {{path/to/file}}
```
#### Search for a pattern in all files recursively in a directory, showing line numbers of matches, ignoring binary files:
```shell
grep --recursive --line-number --binary-files={{without-match}} "{{search_pattern}}" {{path/to/directory}}
```
#### Use extended regular expressions (supports `?`, `+`, `{}`, `()` and `|`), in case-insensitive mode:
```shell
grep --extended-regexp --ignore-case "{{search_pattern}}" {{path/to/file}}
```
#### Print 3 lines of context around, before, or after each match:
```shell
grep --{{context|before-context|after-context}}={{3}} "{{search_pattern}}" {{path/to/file}}
```
#### Print file name and line number for each match:
```shell
grep --with-filename --line-number "{{search_pattern}}" {{path/to/file}}
```
#### Search for lines matching a pattern, printing only the matched text:
```shell
grep --only-matching "{{search_pattern}}" {{path/to/file}}
```
#### Search stdin for lines that do not match a pattern:
```shell
cat {{path/to/file}} | grep --invert-match "{{search_pattern}}"
```
{% endraw %}