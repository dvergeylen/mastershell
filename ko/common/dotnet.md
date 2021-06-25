---
layout: default
title: "dotnet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dotnet">
  <a href="/ko/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> .NET Core를 위한 크로스 플랫폼 .NET 명령어 도구.
> 더 많은 정보: <https://docs.microsoft.com/dotnet/core/tools>.

#### 새 .NET 프로젝트 초기화하기:
```shell
dotnet new {{짧은_템플릿_이름}}
```
#### nuget 패키지들 복구하기:
```shell
dotnet restore
```
#### 현재 디렉토리에서 .NET 프로젝트를 빌드하고 실행하기:
```shell
dotnet run
```
#### 패키지화 된 dotnet 어플리케이션을 실행하기(런타임만 필요하며, 나머지 명령어들은 .NET Core SDK 설치가 필요):
```shell
dotnet {{경로/어플리케이션.dll}}
```
{% endraw %}