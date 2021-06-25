---
layout: default
title: "cradle elastic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-elastic">
  <a href="/ko/common/cradle-elastic.html">cradle elastic</a> <a href="#cradle-elastic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cradle 인스턴스의 ElasticSearch 인스턴스 관리.
> 더 많은 정보: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#elastic>.

#### ElasticSearch 색인 자르기:
```shell
cradle elastic flush
```
#### 특정 패키지에 대한 ElasticSearch 색인 자르기:
```shell
cradle elastic flush {{패키지_명}}
```
#### ElasticSearch 스키마 제출:
```shell
cradle elastic map
```
#### 특정 패키지에 대한 ElasticSearch 스키마 제출:
```shell
cradle elastic map {{패키지_명}}
```
#### 모든 패키지에 대한 ElasticSearch 색인 채우기:
```shell
cradle elastic populate
```
#### 특정 패키지에 대한 ElasticSearch 색인 채우기:
```shell
cradle elastic populate {{패키지_명}}
```
{% endraw %}