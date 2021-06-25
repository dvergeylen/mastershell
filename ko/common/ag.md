---
layout: default
title: "ag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ag">
  <a href="/ko/common/ag.html">ag</a> <a href="#ag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Silver Searcher.
> ack과 비슷하지만, 더 빠르다.
> 더 많은 정보: <https://github.com/ggreer/the_silver_searcher>.

#### "foo"를 포함하고 있는 파일들을 찾고, 내용에서 일치하는 행을 출력:
```shell
ag {{foo}}
```
#### 특정 디렉토리에서 "foo"를 포함하고 있는 파일 찾기:
```shell
ag {{foo}} {{경로/디렉토리명}}
```
#### "foo"를 포함하고 있는 파일을 찾되, 파일 이름만 나열:
```shell
ag -l {{foo}}
```
#### "FOO"를 포함하고 있는 파일들을 사례별로 찾고, 전체 라인이 아닌 일치 라인만 인쇄:
```shell
ag -i -o {{FOO}}
```
#### "bar" 제목과 일치하는 파일에서 "foo" 찾기:
```shell
ag {{foo}} -G {{bar}}
```
#### 내용이 정규식과 일치하는 파일 찾기:
```shell
ag '{{^ba(r|z)$}}'
```
#### 이름이 "foo"와 일치하는 파일 찾기:
```shell
ag -g {{foo}}
```
{% endraw %}