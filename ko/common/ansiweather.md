---
layout: default
title: "ansiweather"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansiweather">
  <a href="/ko/common/ansiweather.html">ansiweather</a> <a href="#ansiweather"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 당신의 터미널에서 현재 날씨 상태를 표시하는 쉘 스크립트.
> 더 많은 정보: <https://github.com/fcambus/ansiweather>.

#### 폴란드 르제조에 대한 메트릭 단위를 사용하여 예측 표시:
```shell
ansiweather -u {{metric}} -f {{5}} -l {{Rzeszow,PL}}
```
#### 당신의 현재 위치에 대한 기호 및 일광 데이터를 표시하는 예측 표시:
```shell
ansiweather -s {{true}} -d {{true}}
```
#### 당신의 현재 위치의 바람과 습도 데이터를 보여주는 예측 표시:
```shell
ansiweather -w {{true}} -h {{true}}
```
{% endraw %}