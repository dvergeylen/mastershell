---
layout: default
title: "cmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmd">
  <a href="/de/android/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Androids Service-Manager.
> Weitere Informationen: <https://cs.android.com/android/platform/superproject/+/master:frameworks/native/cmds/cmd/>.

#### Liste alle laufenden Services auf:
```shell
cmd -l
```
#### Rufe einen bestimmten Service auf:
```shell
cmd {{alarm}}
```
#### Rufe einen bestimmten Service mit Parametern auf:
```shell
cmd {{vibrator}} {{vibrate 300}}
```
{% endraw %}