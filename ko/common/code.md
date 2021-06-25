---
layout: default
title: "code"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="code">
  <a href="/ko/common/code.html">code</a> <a href="#code"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 비주얼 스튜디오 코드.
> 더 많은 정보: <https://github.com/microsoft/vscode>.

#### VS Code 열기:
```shell
code
```
#### 현재 디렉토리에서 VS Code 열기:
```shell
code .
```
#### 파일이나 디렉토리에서 VS Code 열기:
```shell
code {{경로/파일_혹은_디렉토리}}
```
#### 현재 열려 있는 VS 코드 창에서 파일 또는 디렉토리를 열기:
```shell
code --reuse-window {{경로/파일_혹은_디렉토리}}
```
#### 두 개의 VS Code 파일 비교:
```shell
code -d {{파일1}} {{파일2}}
```
{% endraw %}