---
layout: default
title: "convmv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="convmv">
  <a href="/ko/common/convmv.html">convmv</a> <a href="#convmv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 한 인코딩에서 다른 인코딩으로 파일 이름(파일 내용 X)을 변환.
> 더 많은 정보: <https://www.j3e.de/linux/convmv/man/>.

#### 파일 이름 인코딩 변환 테스트(파일 이름을 실제로 변경하지 마십시오):
```shell
convmv -f {{인코딩_에서}} -t {{인코딩_으로}} {{입력_파일}}
```
#### 파일 이름 인코딩을 변환하고 파일 이름을 새 인코딩으로 변환:
```shell
convmv -f {{인코딩_에서}} -t {{인코딩_으로}} --notest {{입력_파일}}
```
{% endraw %}