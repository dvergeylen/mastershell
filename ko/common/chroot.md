---
layout: default
title: "chroot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chroot">
  <a href="/ko/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 특수 루트 디렉토리를 사용하여 명령 또는 대화형 쉘 실행.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/chroot>.

#### 새로운 루트 디렉토리로 명령어 실행:
```shell
chroot {{/경로/새로운/루트/디렉토리}} {{명령어}}
```
#### 사용할 사용자 및 그룹(ID 또는 이름) 지정:
```shell
chroot --userspec={{사용자:그룹}}
```
{% endraw %}