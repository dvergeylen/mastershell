---
layout: default
title: "ansible-galaxy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-galaxy">
  <a href="/ko/common/ansible-galaxy.html">ansible-galaxy</a> <a href="#ansible-galaxy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 수용 가능한 역할 생성 및 관리.
> 더 많은 정보: <https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html>.

#### 역할 설치:
```shell
ansible-galaxy install {{사용자이름.역할_}}
```
#### 역할 제거:
```shell
ansible-galaxy remove {{사용자이름.역할_이름}}
```
#### 설치된 역할 리스트:
```shell
ansible-galaxy list
```
#### 주어진 역할에 대해 검색:
```shell
ansible-galaxy search {{역할_이름}}
```
#### 새로운 역할 생성:
```shell
ansible-galaxy init {{역할_이름}}
```
{% endraw %}