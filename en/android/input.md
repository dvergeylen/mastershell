---
layout: default
title: "input"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="input">
  <a href="/en/android/input.html">input</a> <a href="#input"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send event codes or touchscreen gestures to an Android device.
> This command can only be used through `adb shell`.
> More information: <https://developer.android.com/reference/android/view/KeyEvent.html#constants_1>.

#### Send an event code for a single character to an Android device:
```shell
input keyevent {{event_code}}
```
#### Send a text to an Android device (`%s` represents spaces):
```shell
input text "{{text}}"
```
#### Send a single tap to an Android device:
```shell
input tap {{x_pos}} {{y_pos}}
```
#### Send a swipe gesture to an Android device:
```shell
input swipe {{x_start}} {{y_start}} {{x_end}} {{y_end}} {{duration_in_ms}}
```
#### Send a long press to an Android device using a swipe gesture:
```shell
input swipe {{x_pos}} {{y_pos}} {{x_pos}} {{y_pos}} {{duration_in_ms}}
```
{% endraw %}