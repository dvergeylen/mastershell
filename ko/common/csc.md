---
layout: default
title: "csc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csc">
  <a href="/ko/common/csc.html">csc</a> <a href="#csc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 마이크로 소프트 사의 C# 컴파일러.
> 더 많은 정보: <https://docs.microsoft.com/dotnet/csharp/language-reference/compiler-options/command-line-building-with-csc-exe>.

#### 하나 이상의 C# 파일을 CIL 실행파일로 컴파일:
```shell
csc {{경로/입력파일_a.cs}} {{경로/입력파일_b.cs}}
```
#### 출력 파일 이름 지정:
```shell
csc /out:{{경로/파일명}} {{경로/입력파일.cs}}
```
#### 실행 파일 대신 '.dll' 라이브러리로 컴파일:
```shell
csc /target:library {{경로/입력파일.cs}}
```
#### 다른 어셈블리 참조:
```shell
csc /reference:{{경로/라이브러리.dll}} {{경로/입력파일.cs}}
```
#### 리소스 포함:
```shell
csc /resource:{{경로/리소스파일}} {{경로/입력파일.cs}}
```
#### XML 문서 자동 생성:
```shell
csc /doc:{{경로/출력파일.xml}} {{경로/입력파일.cs}}
```
#### 아이콘 지정:
```shell
csc /win32icon:{{경로/아이콘.ico}} {{경로/입력파일.cs}}
```
#### 키 파일을 사용하여 결과 어셈블리의 이름 지정:
```shell
csc /keyfile:{{경로/키파일}} {{경로/입력파일.cs}}
```
{% endraw %}