---
layout: default
title: "btrfs scrub"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btrfs-scrub">
  <a href="/zh/linux/btrfs-scrub.html">btrfs scrub</a> <a href="#btrfs-scrub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 清理 btrfs 文件系统以验证数据完整性。
> 建议每月运行一次 scrub。
> 更多信息：<https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-scrub>。

#### 开始 scrub：
```shell
sudo btrfs scrub start {{指向挂载点的路径}}
```
#### 显示正在进行或上次完成的 scrub 的状态：
```shell
sudo btrfs scrub status {{指向挂载点的路径}}
```
#### 取消正在进行的 scrub：
```shell
sudo btrfs scrub cancel {{指向挂载点的路径}}
```
#### 恢复先前取消的 scrub：
```shell
sudo btrfs scrub resume {{指向挂载点的路径}}
```
#### 开始擦洗，但要等到 scrub 完成后才能退出：
```shell
sudo btrfs scrub start -B {{指向挂载点的路径}}
```
#### 在安静模式下启动 scrub（不打印错误或统计信息）：
```shell
sudo btrfs scrub start -q {{指向挂载点的路径}}
```
{% endraw %}