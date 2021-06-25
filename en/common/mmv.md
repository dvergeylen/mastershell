---
layout: default
title: "mmv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mmv">
  <a href="/en/common/mmv.html">mmv</a> <a href="#mmv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Move and rename files in bulk.

#### Rename all files with a certain extension to a different extension:
```shell
mmv "*{{.old_extension}}" "#1{{.new_extension}}"
```
#### Copy `report6part4.txt` to `./french/rapport6partie4.txt` along with all similarly named files:
```shell
mmv -c "{{report*part*.txt}}" "{{./french/rapport#1partie#2.txt}}"
```
#### Append all `.txt` files into one file:
```shell
mmv -a "{{*.txt}}" "{{all.txt}}"
```
#### Convert dates in filenames from "M-D-Y" format to "D-M-Y" format:
```shell
mmv "{{[0-1][0-9]-[0-3][0-9]-[0-9][0-9][0-9][0-9].txt}}" "{{#3#4-#1#2-#5#6#7#8.txt}}"
```
{% endraw %}