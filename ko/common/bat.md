---
layout: default
title: "bat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bat">
  <a href="/ko/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 파일들을 출력하고 연결. 구문 강조와 Git 통합을 가진`cat`클론.

#### 파일 내용을 표준 출력으로 출력:
```shell
bat {{file}}
```
#### 여러 파일을 대상 파일에 연결:
```shell
bat {{file1}} {{file2}} > {{target_file}}
```
#### 대상 파일에 여러 파일을 추가:
```shell
bat {{file1}} {{file2}} >> {{target_file}}
```
#### 모든 출력 라인 번호 매기기:
```shell
bat -n {{file}}
```
#### json파일 구문 강조:
```shell
bat --language json {{file.json}}
```
#### 지원되는 모든 언어 표시:
```shell
bat --list-languages
```
{% endraw %}