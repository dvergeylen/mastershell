---
layout: default
title: "axel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="axel">
  <a href="/ko/common/axel.html">axel</a> <a href="#axel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 가속기를 다운로드 하십시오. HTTP, HTTPS, FTP를 지원합니다.
> 더 많은 정보: <https://github.com/axel-download-accelerator/axel>.

#### 파일로 URL 다운로드:
```shell
axel {{url}}
```
#### 다운로드 및 파일 이름 지정:
```shell
axel {{url}} -o {{filename}}
```
#### 여러 연결로 다운로드:
```shell
axel -n {{connections_num}} {{url}}
```
#### mirrors 검색:
```shell
axel -S {{mirrors_num}} {{url}}
```
#### 다운로드 속도 제한 (초당 바이트):
```shell
axel -s {{speed}} {{url}}
```
{% endraw %}