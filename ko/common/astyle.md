---
layout: default
title: "astyle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="astyle">
  <a href="/ko/common/astyle.html">astyle</a> <a href="#astyle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> C, C ++, C # 및 Java 프로그래밍 언어에 대한 소스 코드 인덴터, 포맷터 및 미화기.
> 실행 시 원본 파일의 사본은 원래 파일 이름에 ".orig"가 추가된 상태로 작성된다.
> 더 많은 정보: <http://astyle.sourceforge.net/>.

#### 들여쓰기 당 4개의 공백의 기본 스타일을 적용하고 형식 변경 없도록 적용:
```shell
astyle {{소스파일명}}
```
#### java 스타일 코드로 적용:
```shell
astyle --style=java {{경로/파일명}}
```
#### allman 스타일 코드로 적용:
```shell
astyle --style=allman {{경로/파일명}}
```
#### 공간을 사용하여 사용자 지정 들여쓰기를 적용합니다. 2에서 20개 사이의 공간을 선택합니다:
```shell
astyle --indent=spaces={{띄어쓸_수}} {{경로/파일명}}
```
#### 탭을 사용하여 사용자 지정 들여쓰기를 적용합니다. 2에서 20 탭 사이에서 선택합니다:
```shell
astyle --indent=tab={{탭_수}} {{경로/파일명}}
```
{% endraw %}