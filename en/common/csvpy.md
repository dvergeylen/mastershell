---
layout: default
title: "csvpy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvpy">
  <a href="/en/common/csvpy.html">csvpy</a> <a href="#csvpy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Loads a CSV file into a Python shell.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvpy.html>.

#### Load a CSV file into a `CSVKitReader` object:
```shell
csvpy {{data.csv}}
```
#### Load a CSV file into a `CSVKitDictReader` object:
```shell
csvpy --dict {{data.csv}}
```
{% endraw %}