---
layout: default
title: "cmp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmp">
  <a href="/ko/common/cmp.html">cmp</a> <a href="#cmp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 두 개의 파일 비교.
> 더 많은 정보: <https://www.gnu.org/software/diffutils/manual/html_node/Invoking-cmp.html>.

#### 파일 간의 첫 번째 바이트 번호와 선 번호의 차이를 찾습니다:
```shell
cmp {{파일1}} {{파일2}}
```
#### 모든 바이트 수와 다른 바이트의 차이 찾기:
```shell
cmp -l {{파일1}} {{파일2}}
```
{% endraw %}