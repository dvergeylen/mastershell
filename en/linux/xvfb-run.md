---
layout: default
title: "xvfb-run"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xvfb-run">
  <a href="/en/linux/xvfb-run.html">xvfb-run</a> <a href="#xvfb-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a command in a virtual X server environment.
> More information: <https://www.x.org/wiki/>.

#### Run the specified command in a virtual X server:
```shell
xvfb-run {{command}}
```
#### Try to get a free server number, if the default (99) is not available:
```shell
xvfb-run --auto-servernum {{command}}
```
#### Pass arguments to the Xvfb server:
```shell
xvfb-run --server-args "{{-screen 0 1024x768x24}}" {{command}}
```
{% endraw %}