---
layout: default
title: "am"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="am">
  <a href="/zh/android/am.html">am</a> <a href="#am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android 活动管理器。
> 更多信息见：<https://developer.android.com/studio/command-line/adb#am>.

#### 启动一个指定的活动：
```shell
am start -n {{com.android.settings/.Settings}}
```
#### 启动一个活动并将数据传递给它：
```shell
am start -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
#### 启动与特定操作和类别匹配的活动：
```shell
am start -a {{android.intent.action.MAIN}} -c {{android.intent.category.HOME}}
```
#### 将意图转换为 URI：
```shell
am to-uri -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
{% endraw %}