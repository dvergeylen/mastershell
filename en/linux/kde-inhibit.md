---
layout: default
title: "kde-inhibit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kde-inhibit">
  <a href="/en/linux/kde-inhibit.html">kde-inhibit</a> <a href="#kde-inhibit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inhibit various desktop functions while a command runs.

#### Inhibit power management:
```shell
kde-inhibit --power {{command}} {{command_arguments}}
```
#### Inhibit screen saver:
```shell
kde-inhibit --screenSaver {{command}} {{command_arguments}}
```
#### Launch vlc, and inhibit colour correction (night mode) while it's running:
```shell
kde-inhibit --colorCorrect {{vlc}}
```
{% endraw %}