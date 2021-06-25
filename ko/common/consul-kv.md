---
layout: default
title: "consul-kv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="consul-kv">
  <a href="/ko/common/consul-kv.html">consul-kv</a> <a href="#consul-kv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 서비스 검색 기능과 상태 확인을 위한 분산된 키-값(key-value)쌍 저장.
> 더 많은 정보: <https://learn.hashicorp.com/consul/getting-started/kv>.

#### 키-값(key-value)쌍으로 저장된 값 읽기:
```shell
consul kv get {{키}}
```
#### 새로운 키-값(key-value)쌍으로 저장:
```shell
consul kv put {{키}} {{값}}
```
#### 키-값(key-value)쌍 제거:
```shell
consul kv delete {{키}}
```
{% endraw %}