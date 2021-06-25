---
layout: default
title: "choco pack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-pack">
  <a href="/zh/windows/choco-pack.html">choco pack</a> <a href="#choco-pack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 nuspec 打包到已编译的 nupkg.

#### 将 nuspec 打包到已编译的 nupkg:
```shell
choco pack {{nuspec 的路径}}
```
#### 将 nuspec 打包到已编译的 nupkg, 并指定生成的版本:
```shell
choco pack {{nuspec 的路径}} --version {{版本号}}
```
#### 将 nuspec 打包到已编译的 nupkg, 并输出到指定的目录:
```shell
choco pack {{nuspec 的路径}} --output-directory {{输出目录的路径}}
```
{% endraw %}