---
layout: default
title: "screenkey"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="screenkey">
  <a href="/en/linux/screenkey.html">screenkey</a> <a href="#screenkey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A screencast tool to display keys pressed.
> More information: <https://www.thregr.org/~wavexx/software/screenkey/>.

#### Display keys which are currently being pressed on the screen:
```shell
screenkey
```
#### Display keys and mouse buttons which are currently being pressed on the screen:
```shell
screenkey --mouse
```
#### Launch the settings menu of screenkey:
```shell
screenkey --show-settings
```
#### Launch screenkey at a specific position:
```shell
screenkey --position {{top|center|bottom|fixed}}
```
#### Change the format of the key modifiers displayed on screen:
```shell
screenkey --mods-mode {{normal|emacs|mac|win|tux}}
```
#### Change the appearance of screenkey:
```shell
screenkey --bg-color "{{#a1b2c3}}" --font {{Hack}} --font-color {{yellow}} --opacity {{0.8}}
```
#### Drag and select a window on screen to display screenkey:
```shell
screenkey --position fixed --geometry {{$(slop -n -f '%g')}}
```
{% endraw %}