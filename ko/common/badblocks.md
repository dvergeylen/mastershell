---
layout: default
title: "badblocks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="badblocks">
  <a href="/ko/common/badblocks.html">badblocks</a> <a href="#badblocks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 불량 블록이 있는지 장치를 검사하십시오.
> 불량 블록을 사용하면 파티션 테이블을 포함하여 디스크의 모든 데이터를 지우는 등의 파괴적인 작업이 발생할 수 있습니다.
> 더 많은 정보: <https://manned.org/badblocks>.

#### 비파괴 읽기 전용 테스트를 사용하여 디스크에서 불량 블록을 검사:
```shell
sudo badblocks {{/dev/sda}}
```
#### 비파괴 읽기-쓰기 테스트로 마운트되지 않은 디스크에서 불량 블록이 있는지 검사:
```shell
sudo badblocks -n {{/dev/sda}}
```
#### 파괴 쓰기 테스트로 마운드되지 않은 디스크에서 불량 블록이 있는지 검사:
```shell
sudo badblocks -w {{/dev/sda}}
```
{% endraw %}