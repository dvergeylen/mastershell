---
layout: default
title: "cmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmd">
  <a href="/en/android/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android service manager.
> More information: <https://cs.android.com/android/platform/superproject/+/master:frameworks/native/cmds/cmd/>.

#### List every running service:
```shell
cmd -l
```
#### Call a specific service:
```shell
cmd {{alarm}}
```
#### Call a service with arguments:
```shell
cmd {{vibrator}} {{vibrate 300}}
```
{% endraw %}