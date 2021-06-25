---
layout: default
title: "chgrp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chgrp">
  <a href="/ko/common/chgrp.html">chgrp</a> <a href="#chgrp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 파일 및 디렉토리의 그룹 소유권 변경.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/chgrp>.

#### 파일/디렉토리의 소유 그룹 변경:
```shell
chgrp {{그룹}} {{경로/파일명_또는_디렉토리명}}
```
#### 디렉토리 및 해당 컨텐츠의 소유 그룹 변경:
```shell
chgrp -R {{그룹}} {{경로/디렉토리명}}
```
#### 심볼릭 링크의 소유 그룹 변경:
```shell
chgrp -h {{그룹}} {{경로/심볼릭_링크}}
```
#### 참조 파일과 일치하도록 파일/디렉토리의 소유 그룹 변경:
```shell
chgrp --reference={{경로/참조_파일명}} {{경로/파일명_또는_디렉토리명}}
```
{% endraw %}