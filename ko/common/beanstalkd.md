---
layout: default
title: "beanstalkd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="beanstalkd">
  <a href="/ko/common/beanstalkd.html">beanstalkd</a> <a href="#beanstalkd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 단순하고 일반적인 work-queue 서버.
> 더 많은 정보:<https://beanstalkd.github.io/>.

#### beanstalkd를 시작하고, 11300 포트로 듣기:
```shell
beanstalkd
```
#### 사용자가 지정한 포트 및 주소에서 beanstalkd 듣기 시작:
```shell
beanstalkd -l {{ip_address}} -p {{port_number}}
```
#### work queue를 디스크에 저장하고 유지:
```shell
beanstalkd -b {{path/to/persistence_directory}}
```
#### 500밀리초마다 지속성있는 디렉토리에 동기화:
```shell
beanstalkd -b {{path/to/persistence_directory}} -f {{500}}
```
{% endraw %}