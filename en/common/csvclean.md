---
layout: default
title: "csvclean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvclean">
  <a href="/en/common/csvclean.html">csvclean</a> <a href="#csvclean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Finds and cleans common syntax errors in CSV files.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvclean.html>.

#### Clean a CSV file:
```shell
csvclean {{bad.csv}}
```
#### List locations of syntax errors in a CSV file:
```shell
csvclean -n {{bad.csv}}
```
{% endraw %}