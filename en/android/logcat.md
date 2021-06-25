---
layout: default
title: "logcat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logcat">
  <a href="/en/android/logcat.html">logcat</a> <a href="#logcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dump a log of system messages.
> More information: <https://developer.android.com/studio/command-line/logcat>.

#### Display system logs:
```shell
logcat
```
#### Write system logs to a file:
```shell
logcat -f {{path/to/file}}
```
#### Display lines that match a regular expression:
```shell
logcat --regex {{regular_expression}}
```
{% endraw %}