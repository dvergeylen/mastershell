---
layout: default
title: "csvkit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvkit">
  <a href="/en/common/csvkit.html">csvkit</a> <a href="#csvkit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manipulation toolkit for CSV files.
> See the individual commands: `csvclean`, `csvcut`, `csvformat`, `csvgrep`, `csvlook`, `csvpy`, `csvsort`, `csvstat`.
> More information: <https://csvkit.readthedocs.io/en/0.9.1/cli.html>.

#### Run a command on a CSV file with a custom delimiter:
```shell
{{cmd}} -d {{delimiter}} {{filename.csv}}
```
#### Run a command on a CSV file with a tab as a delimiter (overrides -d):
```shell
{{cmd}} -t {{filename.csv}}
```
#### Run a command on a CSV file with a custom quote character:
```shell
{{cmd}} -q {{quote_char}} {{filename.csv}}
```
#### Run a command on a CSV file with no header row:
```shell
{{cmd}} -H {{filename.csv}}
```
{% endraw %}