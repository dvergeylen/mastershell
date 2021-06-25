---
layout: default
title: "batch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="batch">
  <a href="/ko/common/batch.html">batch</a> <a href="#batch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 시스템 로드 레벨이 허가된 후, 명령을 실행하십시오. 실제로 실행하기 위해서는 atd (혹은 atrun) 를 실행해야합니다.
> 더 많은 정보: <https://man.archlinux.org/man/at.1>.

#### 표준 입력에서 명령 실행하기 (완료 시 `Ctrl + D` 를 누릅니다):
```shell
batch
```
#### 표준 입력에서의 명령 실행하기:
```shell
echo "{{./make_db_backup.sh}}" | batch
```
#### 특정 파일에서 명령 실행하기:
```shell
batch -f {{path/to/file}}
```
{% endraw %}