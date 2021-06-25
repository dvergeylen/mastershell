---
layout: default
title: "rmdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rmdir">
  <a href="/zh_tw/common/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 移除目錄。
> 更多資訊： <https://www.gnu.org/software/coreutils/rmdir>.

#### 若為空目錄則移除目錄（如果目錄非空，可用 `rm -r` 移除目錄及其所包含的檔案）：
```shell
rmdir {{目錄/完整/路徑}}
```
#### 移除目錄與其所有上層目錄：
```shell
rmdir -p {{目錄/完整/路徑}}
```
{% endraw %}