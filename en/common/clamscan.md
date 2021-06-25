---
layout: default
title: "clamscan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clamscan">
  <a href="/en/common/clamscan.html">clamscan</a> <a href="#clamscan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line virus scanner.
> More information: <https://www.clamav.net>.

#### Scan a file for vulnerabilities:
```shell
clamscan {{path/to/file}}
```
#### Scan all files recursively in a specific directory:
```shell
clamscan -r {{path/to/directory}}
```
#### Scan data from stdin:
```shell
{{command}} | clamscan -
```
#### Specify a virus database file or directory of files:
```shell
clamscan --database {{path/to/database_file_or_directory}}
```
#### Scan the current directory and output only infected files:
```shell
clamscan --infected
```
#### Output the scan report to a log file:
```shell
clamscan --log {{path/to/log_file}}
```
#### Move infected files to a specific directory:
```shell
clamscan --move {{path/to/quarantine_directory}}
```
#### Remove infected files:
```shell
clamscan --remove yes
```
{% endraw %}