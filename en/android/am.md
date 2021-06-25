---
layout: default
title: "am"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="am">
  <a href="/en/android/am.html">am</a> <a href="#am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android activity manager.
> More information: <https://developer.android.com/studio/command-line/adb#am>.

#### Start a specific activity:
```shell
am start -n {{com.android.settings/.Settings}}
```
#### Start an activity and pass data to it:
```shell
am start -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
#### Start an activity matching a specific action and category:
```shell
am start -a {{android.intent.action.MAIN}} -c {{android.intent.category.HOME}}
```
#### Convert an intent to an URI:
```shell
am to-uri -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
{% endraw %}