---
layout: default
title: "cmark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmark">
  <a href="/ko/common/cmark.html">cmark</a> <a href="#cmark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CommonMark Markdown 텍스트를 다른 텍스트 형식으로 변환합니다.
> 더 많은 정보: <https://github.com/commonmark/cmark>.

#### CommonMark Markdown 파일을 HTML 파일로 렌더링합니다:
```shell
cmark --to html {{파일명.md}}
```
#### 데이터를 표준 입력에서 라텍스로 변환:
```shell
cmark --to latex
```
#### 직선 따옴표를 스마트 따옴표로 변환:
```shell
cmark --smart --to html {{파일명.md}}
```
#### UTF-8 문자들을 검증:
```shell
cmark --validate-utf8 {{파일명.md}}
```
{% endraw %}