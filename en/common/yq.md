---
layout: default
title: "yq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yq">
  <a href="/en/common/yq.html">yq</a> <a href="#yq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A lightweight and portable command-line YAML processor.
> More information: <https://mikefarah.gitbook.io/yq/>.

#### Output a YAML file, in pretty-print format (v4+):
```shell
yq eval {{path/to/file.yaml}}
```
#### Output a YAML file, in pretty-print format (v3):
```shell
yq read {{path/to/file.yaml}} --colors
```
#### Output the first element in a YAML file that contains only an array (v4+):
```shell
yq eval '.[0]' {{path/to/file.yaml}}
```
#### Output the first element in a YAML file that contains only an array (v3):
```shell
yq read {{path/to/file.yaml}} '[0]'
```
#### Set (or overwrite) a key to a value in a file (v4+):
```shell
yq eval '.{{key}} = "{{value}}"' --inplace {{path/to/file.yaml}}
```
#### Set (or overwrite) a key to a value in a file (v3):
```shell
yq write --inplace {{path/to/file.yaml}} '{{key}}' '{{value}}'
```
#### Merge two files and print to stdout (v4+):
```shell
yq eval-all 'select(filename == "{{path/to/file1.yaml}}") * select(filename == "{{path/to/file2.yaml}}")' {{path/to/file1.yaml}} {{path/to/file2.yaml}}
```
#### Merge two files and print to stdout (v3):
```shell
yq merge {{path/to/file1.yaml}} {{path/to/file2.yaml}} --colors
```
{% endraw %}