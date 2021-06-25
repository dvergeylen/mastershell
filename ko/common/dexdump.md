---
layout: default
title: "dexdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dexdump">
  <a href="/ko/common/dexdump.html">dexdump</a> <a href="#dexdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 안드로이드 DEX 파일들에 대한 정보 출력.
> 더 많은 정보: <https://manpages.ubuntu.com/manpages/latest/en/man1/dexdump.1.html>.

#### APK 파일으로부터 클래스들과 메서드들 추출:
```shell
dexdump {{경로/파일명.apk}}
```
#### APK 파일에 포함된 DEX 파일들의 헤더 정보 출력:
```shell
dexdump -f {{경로/파일명.apk}}
```
#### 실행가능한 섹션의 분해된 결과 출력:
```shell
dexdump -d {{경로/파일명.apk}}
```
#### 파일로 결과 출력:
```shell
dexdump -o {{경로/파일명}} {{경로/파일명.apk}}
```
{% endraw %}