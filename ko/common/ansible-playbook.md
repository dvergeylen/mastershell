---
layout: default
title: "ansible-playbook"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-playbook">
  <a href="/ko/common/ansible-playbook.html">ansible-playbook</a> <a href="#ansible-playbook"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SSH를 통해 원격 머신에서 playbook에 정의된 작업 실행.
> 더 많은 정보: <https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html>.

#### playbook에서 작업 실행:
```shell
ansible-playbook {{playbook}}
```
#### 사용자 정의 호스트 인벤토리를 포함한 playbook에서 작업 실행:
```shell
ansible-playbook {{playbook}} -i {{인벤토리_파일}}
```
#### 명령어 라인을 통해 정의된 추가 변수를 사용하여 playbook에서 작업 실행:
```shell
ansible-playbook {{playbook}} -e "{{변수1}}={{값1}} {{변수2}}={{값2}}"
```
#### json 파일에 정의된 추가 변수를 사용하여 playbook에서 작업 실행:
```shell
ansible-playbook {{playbook}} -e "@{{변수.json}}"
```
{% endraw %}