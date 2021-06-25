---
layout: default
title: "xfce4-screenshooter"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xfce4-screenshooter">
  <a href="/en/linux/xfce4-screenshooter.html">xfce4-screenshooter</a> <a href="#xfce4-screenshooter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The XFCE4 screenshot tool.
> More information: <https://docs.xfce.org/apps/xfce4-screenshooter/start>.

#### Launch the screenshooter GUI:
```shell
xfce4-screenshooter
```
#### Take a screenshot of the entire screen and launch the GUI to ask how to proceed:
```shell
xfce4-screenshooter --fullscreen
```
#### Take a screenshot of the entire screen and save it in the specified directory:
```shell
xfce4-screenshooter --fullscreen --save {{path/to/directory}}
```
#### Wait some time before taking the screenshot:
```shell
xfce4-screenshooter --delay {{seconds}}
```
#### Take a screenshot of a region of the screen (select using the mouse):
```shell
xfce4-screenshooter --region
```
#### Take a screenshot of the active window, and copy it to the clipboard:
```shell
xfce4-screenshooter --window --clipboard
```
#### Take a screenshot of the active window, and open it with a chosen program:
```shell
xfce4-screenshooter --window --open {{gimp}}
```
{% endraw %}