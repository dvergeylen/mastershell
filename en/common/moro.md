---
layout: default
title: "moro"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="moro">
  <a href="/en/common/moro.html">moro</a> <a href="#moro"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Track work time.
> More information: <https://moro.js.org>.

#### Invoke `moro` without parameters, to set the current time as the start of the working day:
```shell
moro
```
#### Specify a custom time for the start of the working day:
```shell
moro hi {{09:30}}
```
#### Invoke `moro` without parameters a second time, to set the current time at the end of the working day:
```shell
moro
```
#### Specify a custom time for the end of the working day:
```shell
moro bye {{17:30}}
```
#### Add a note on the current working day:
```shell
moro note {{3 hours on project Foo}}
```
#### Show a report of time logs and notes for the current working day:
```shell
moro report
```
#### Show a report of time logs and notes for all working days on record:
```shell
moro report --all
```
{% endraw %}