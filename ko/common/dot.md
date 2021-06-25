---
layout: default
title: "dot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dot">
  <a href="/ko/common/dot.html">dot</a> <a href="#dot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 방향 그래프의 레이어 도면을 생성하는 명령 도구입니다.
> 더 많은 정보: <https://www.graphviz.org/pdf/dotguide.pdf>.

#### 입력 파일 이름과 선택한 포맷을 기반으로 이미지 파일을 랜더링하고 출력파일 이름 결정하기:
```shell
dot -Tpng -O {{경로/파일명.dot}}
```
#### DOT 파일로부터 SVG 생성하기:
```shell
dot -Tsvg -o {{경로/출력_파일명.svg}} {{경로/파일명.dot}}
```
{% endraw %}