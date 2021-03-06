---
layout: default
title: "convert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="convert">
  <a href="/ko/common/convert.html">convert</a> <a href="#convert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ImageMagick 이미지 변환 도구.
> 더 많은 정보: <https://imagemagick.org/script/convert.php>.

#### JPG이미지를 PNG이미지로 변환:
```shell
convert {{이미지.jpg}} {{이미지.png}}
```
#### 이미지를 원래 크기의 50%로 조정:
```shell
convert {{이미지.png}} -resize 50% {{이미지2.png}}
```
#### 원래 종횡비를 유지하면서 이미지를 최대 640x480 크기로 조정:
```shell
convert {{이미지.png}} -resize 640x480 {{이미지2.png}}
```
#### 이미지를 가로로 추가:
```shell
convert {{이미지1.png}} {{이미지2.png}} {{이미지3.png}} +append {{이미지123.png}}
```
#### 이미지를 세로로 추가:
```shell
convert {{이미지1.png}} {{이미지2.png}} {{이미지3.png}} -append {{이미지123.png}}
```
#### 100ms 지연된 일련의 이미지에서 GIF 만들기:
```shell
convert {{이미지1.png}} {{이미지2.png}} {{이미지3.png}} -delay {{100}} {{애니메이션.gif}}
```
#### 단색 배경만으로 이미지 만들기:
```shell
convert -size {{800x600}} "xc:{{#ff0000}}" {{이미지.png}}
```
{% endraw %}