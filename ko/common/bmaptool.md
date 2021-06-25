---
layout: default
title: "bmaptool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bmaptool">
  <a href="/ko/common/bmaptool.html">bmaptool</a> <a href="#bmaptool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 블록 맵을 지능적으로 생성 및 복사( `cp` 혹은 `dd`보다 빠른 속도).
> 더 많은 정보: <https://source.tizen.org/documentation/reference/bmaptool>.

#### 이미지 파일에서 블록 맵 생성:
```shell
bmaptool create -o {{블록맵.bmap}} {{이미지 파일}}
```
#### 이미지 파일을 sdb로 복사:
```shell
bmaptool copy --bmap {{블록맵.bmap}} {{이미지 파일}} {{/dev/sdb}}
```
#### 압축된 이미지 파일을 sdb로 복사:
```shell
bmaptool copy --bmap {{블록맵.bmap}} {{압축된 이미지 파일}} {{/dev/sdb}}
```
#### 블록맵을 사용하지 않고 이미지 파일을 sdb로 복사:
```shell
bmaptool copy --nobmap {{이미지 파일}} {{/dev/sdb}}
```
{% endraw %}