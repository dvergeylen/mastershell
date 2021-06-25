---
layout: default
title: "basename"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="basename">
  <a href="/ko/common/basename.html">basename</a> <a href="#basename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 경로명의 디렉토리가 아닌 부분을 반환.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/basename>.

#### 경로에서 파일 이름만 표시:
```shell
basename {{path/to/file}}
```
#### 경로에서 접미사가 제거된 파일 이름만 표시:
```shell
basename {{path/to/file}} {{suffix}}
```
{% endraw %}