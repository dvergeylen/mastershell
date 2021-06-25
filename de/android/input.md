---
layout: default
title: "input"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="input">
  <a href="/de/android/input.html">input</a> <a href="#input"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sende Eventcodes oder Touchscreengesten an ein Android-Gerät.
> Dieser Befehl kann nur mit `adb shell` verwendet werden.
> Weitere Informationen: <https://developer.android.com/reference/android/view/KeyEvent.html#constants_1>.

#### Sende einen Eventcode für die Eingabe eines einzelnen Zeichens an ein Gerät:
```shell
input keyevent {{eventcode}}
```
#### Sende einen Text an ein Gerät (`%s` wird als Leerzeichen verwendet):
```shell
input text "{{text}}"
```
#### Sende ein einzelnes Tippen auf den Touchscreen an ein Gerät:
```shell
input tap {{x_pos}} {{y_pos}}
```
#### Sende ein Wischen über den Touchscreen an ein Gerät:
```shell
input swipe {{x_start}} {{y_start}} {{x_ende}} {{y_ende}} {{dauer_in_ms}}
```
#### Sende ein langes Tippen auf den Touschscreen an ein Gerät:
```shell
input swipe {{x_pos}} {{y_pos}} {{x_pos}} {{y_pos}} {{dauer_in_ms}}
```
{% endraw %}