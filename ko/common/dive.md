---
layout: default
title: "dive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dive">
  <a href="/ko/common/dive.html">dive</a> <a href="#dive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 도커 이미지, 레이어 컨텐츠, 그리고 축소 방법 탐색을 위한 도구.
> 더 많은 정보: <https://github.com/wagoodman/dive>.

#### 도커 이미지 분석하기:
```shell
dive {{이미지_태그}}
```
#### 이미지 구축과 분석 시작하기:
```shell
dive build -t {{몇_가지_태그}}
```
{% endraw %}