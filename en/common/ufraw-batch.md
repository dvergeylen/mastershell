---
layout: default
title: "ufraw-batch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ufraw-batch">
  <a href="/en/common/ufraw-batch.html">ufraw-batch</a> <a href="#ufraw-batch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert RAW files from cameras into standard image files.

#### Simply convert RAW files to jpg:
```shell
ufraw-batch --out-type=jpg {{input_file(s)}}
```
#### Simply convert RAW files to png:
```shell
ufraw-batch --out-type=png {{input_file(s)}}
```
#### Extract the preview image from the raw file:
```shell
ufraw-batch --embedded-image {{input_file(s)}}
```
#### Save the file with size up to the given maximums MAX1 and MAX2:
```shell
ufraw-batch --size=MAX1,MAX2 {{input_file(s)}}
```
{% endraw %}