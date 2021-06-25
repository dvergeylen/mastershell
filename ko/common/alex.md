---
layout: default
title: "alex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alex">
  <a href="/ko/common/alex.html">alex</a> <a href="#alex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 민감하지 않고, 사려깊지 않은 글을 잡는 도구.
> 이것은 당신이 선호 성별, 양극화, 인종 관련, 종교에 대한 고려가 불분명하거나 다른 문구가 아닌 문구를 찾는데 도움이 됩니다.
> 더 많은 정보: <https://github.com/get-alex/alex>.

#### stdin으로부터 텍스트 분석:
```shell
echo {{His network looks good}} | alex --stdin
```
#### 현재 디렉토리의 모든 파일 분석:
```shell
alex
```
#### 특정 파일 분석:
```shell
alex {{textfile.md}}
```
#### `example.md`를 제외한 모든 Markdown 파일 분석:
```shell
alex *.md !{{example.md}}
```
{% endraw %}