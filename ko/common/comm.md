---
layout: default
title: "comm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="comm">
  <a href="/ko/common/comm.html">comm</a> <a href="#comm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 두 파일의 공통되는 줄을 선택하거나 거절합니다.
> 두 파일 모두 정렬되어 있어야합니다.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/comm>.

#### 세 개의 탭으로 구분된 열을 생성합니다: 첫 번째 파일에는 줄만, 두 번째 파일에서는 줄들과 공통 줄:
```shell
comm {{파일1}} {{파일2}}
```
#### 두 파일의 공통된 줄들만 출력:
```shell
comm -12 {{파일1}} {{파일2}}
```
#### stdin으로 읽어드린 하나의 파일과 나머지 파일의 공통된 줄들만 출력:
```shell
cat {{파일1}} | comm -12 - {{파일2}}
```
#### 첫 번째 파일에서만 줄을 가져오고 결과를 세 번째 파일에 저장:
```shell
comm -23 {{파일1}} {{파일2}} > {{파일1_only}}
```
#### 파일이 정렬되지 않은 경우 두 번째 파일에서만 줄을 출력합니다:
```shell
comm -13 <(sort {{파일1}}) <(sort {{파일2}})
```
{% endraw %}