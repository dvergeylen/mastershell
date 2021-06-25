---
layout: default
title: "csvpy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvpy">
  <a href="/ko/common/csvpy.html">csvpy</a> <a href="#csvpy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> csvkit에 포함된 CSV 파일을 Python 쉘로 로드.
> 더 많은 정보: <https://csvkit.readthedocs.io/en/latest/scripts/csvpy.html>.

#### CSV 파일을 `CSVKitReader` 오브젝트에 로드:
```shell
csvpy {{데이터.csv}}
```
#### CSV 파일을 `CSVKitDictReader` 오브젝트에 로드:
```shell
csvpy --dict {{데이터.csv}}
```
{% endraw %}