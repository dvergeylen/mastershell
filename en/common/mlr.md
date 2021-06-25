---
layout: default
title: "mlr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mlr">
  <a href="/en/common/mlr.html">mlr</a> <a href="#mlr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Miller is like `awk`, `sed`, `cut`, `join`, and `sort` for name-indexed data such as CSV, TSV, and tabular JSON.
> More information: <https://johnkerl.org/miller/doc>.

#### Pretty-print a CSV file in a tabular format:
```shell
mlr --icsv --opprint cat {{example.csv}}
```
#### Receive JSON data and pretty print the output:
```shell
echo '{"hello":"world"}' | mlr --ijson --opprint cat
```
#### Sort alphabetically on a field:
```shell
mlr --icsv --opprint sort -f {{field}} {{example.csv}}
```
#### Sort in descending numerical order on a field:
```shell
mlr --icsv --opprint sort -nr {{field}} {{example.csv}}
```
#### Convert CSV to JSON, performing calculations and display those calculations:
```shell
mlr --icsv --ojson put '${{newField1}} = ${{oldFieldA}}/${{oldFieldB}}' {{example.csv}}
```
#### Receive JSON and format the output as vertical JSON:
```shell
echo '{"hello":"world", "foo":"bar"}' | mlr --ijson --ojson --jvstack cat
```
#### Filter lines of a compressed CSV file treating numbers as strings:
```shell
mlr --prepipe 'gunzip' --csv filter -S '${{fieldName}} =~ "{{regular_expression}}"' {{example.csv.gz}}
```
{% endraw %}