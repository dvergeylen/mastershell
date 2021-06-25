---
layout: default
title: "notify-send"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="notify-send">
  <a href="/en/linux/notify-send.html">notify-send</a> <a href="#notify-send"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uses the current desktop environment's notification system to create a notification.

#### Show a notification with the title "Test" and the content "This is a test":
```shell
notify-send "{{Test}}" "{{This is a test}}"
```
#### Show a notification with a custom icon:
```shell
notify-send -i {{icon.png}} "{{Test}}" "{{This is a test}}"
```
#### Show a notification for 5 seconds:
```shell
notify-send -t 5000 "{{Test}}" "{{This is a test}}"
```
#### Show a notification with an app's icon:
```shell
notify-send "{{Test}}" --icon={{google-chrome}}
```
{% endraw %}