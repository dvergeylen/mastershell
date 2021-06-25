---
layout: default
title: "csslint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csslint">
  <a href="/ko/common/csslint.html">csslint</a> <a href="#csslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CSS 코드용 린터.
> 더 많은 정보: <https://github.com/CSSLint/csslint/wiki/Command-line-interface>.

#### 하나의 CSS 파일을 린트:
```shell
csslint {{파일.css}}
```
#### 여러개의 CSS 파일을 린트:
```shell
csslint {{파일1.css}} {{파일2.css}} {{파일3.css}}
```
#### 가능한 모든 스타일 규칙 나열:
```shell
csslint --list-rules
```
#### 특정 규칙을 오류로 지정 (종료 코드가 0이아닌 결과로 도출):
```shell
csslint --errors={{에러,보편적-선택자,임포트}} {{파일.css}}
```
#### 특정 규칙을 경고로 지정:
```shell
csslint --warnings={{박스-사이징,선택자-최대값,플롯}} {{파일.css}}
```
#### 완전히 무시할 특정 규칙을 지정:
```shell
csslint --ignore={{ids,규칙-수,속기}} {{파일.css}}
```
{% endraw %}