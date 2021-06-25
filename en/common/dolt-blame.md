---
layout: default
title: "dolt blame"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dolt-blame">
  <a href="/en/common/dolt-blame.html">dolt blame</a> <a href="#dolt-blame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays commit information for each row of a Dolt table.
> More information: <http://github.com/dolthub/dolt>.

#### Display the latest commit for each row of a table:
```shell
dolt blame {{table}}
```
#### Display the latest commits for each row of a table when the specified commit was made:
```shell
dolt blame {{commit}} {{table}}
```
#### View help:
```shell
dolt blame --help
```
{% endraw %}