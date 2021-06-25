---
layout: default
title: "csvclean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvclean">
  <a href="/ko/common/csvclean.html">csvclean</a> <a href="#csvclean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> csvkit에 포함된 CSV 파일의 공통 문법 오류 찾기 및 정리.
> 더 많은 정보: <https://csvkit.readthedocs.io/en/latest/scripts/csvclean.html>.

#### CSV 파일 정리:
```shell
csvclean {{파일.csv}}
```
#### CSV 파일의 문법 오류 위치 나열:
```shell
csvclean -n {{파일.csv}}
```
{% endraw %}