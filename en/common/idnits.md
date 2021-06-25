---
layout: default
title: "idnits"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="idnits">
  <a href="/en/common/idnits.html">idnits</a> <a href="#idnits"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check internet-drafts for submission nits.
> Looks for violations of Section 2.1 and 2.2 of the requirements listed on <https://www.ietf.org/id-info/checklist>.
> More information: <https://tools.ietf.org/tools/idnits/>.

#### Check a file for nits:
```shell
idnits {{path/to/file.txt}}
```
#### Count nits without displaying them:
```shell
idnits --nitcount {{path/to/file.txt}}
```
#### Show extra information about offending lines:
```shell
idnits --verbose {{path/to/file.txt}}
```
#### Expect the specified year in the boilerplate instead of the current year:
```shell
idnits --year {{2021}} {{path/to/file.txt}}
```
#### Assume the document is of the specified status:
```shell
idnits --doctype {{standard|informational|experimental|bcp|ps|ds}} {{path/to/file.txt}}
```
{% endraw %}