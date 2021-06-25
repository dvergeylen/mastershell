---
layout: default
title: "findstr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="findstr">
  <a href="/en/windows/findstr.html">findstr</a> <a href="#findstr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find specified text within one or more files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/findstr>.

#### Find space-separated string(s) in all files:
```shell
findstr "{{query}}" *
```
#### Find space-separated string(s) in a piped command's output:
```shell
{{dir}} | findstr "{{query}}"
```
#### Find space-separated string(s) in all files recur[s]ively:
```shell
findstr /s "{{query}}" *
```
#### Find strings using a case-insensitive search:
```shell
findstr /i "{{query}}" *"
```
#### Find strings in all files using regular expressions:
```shell
findstr /r "{{expression}}" *
```
#### Find a literal string (containing spaces) in all text files:
```shell
findstr /c:"{{query}}" *.txt
```
#### Display the line number before each matching line:
```shell
findstr /n "{{query}}" *
```
#### Display only the filenames that contain a match:
```shell
findstr /m "{{query}}" *
```
{% endraw %}