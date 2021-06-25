---
layout: default
title: "alacritty"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alacritty">
  <a href="/ko/common/alacritty.html">alacritty</a> <a href="#alacritty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 교차 플랫폼으로, GPU-가속 터미널 에뮬레이터.
> 더 많은 정보: <https://github.com/alacritty/alacritty>.

#### 새 Alacritty 창 열기:
```shell
alacritty
```
#### 특정 디렉토리에서 실행:
```shell
alacritty --working-directory {{경로/디렉토리명}}
```
#### 새로운 Alacritty 창에서 명령어 실행:
```shell
alacritty -e {{명령어}}
```
#### 대체 구성파일 지정 (기본값 : `$XDG_CONFIG_HOME/alacritty/alacritty.yml`):
```shell
alacritty --config-file {{경로/config.yml}}
```
#### 재배치가 가능한 라이브 구성 설정으로 실행 (기본적으로 `alacritty.yml` 에서도 활성화 가능):
```shell
alacritty --live-config-reload --config-file {{경로/config.yml}}
```
{% endraw %}