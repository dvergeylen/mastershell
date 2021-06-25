---
layout: default
title: "gotty"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gotty">
  <a href="/en/common/gotty.html">gotty</a> <a href="#gotty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Share your terminal as a web application.
> More information: <https://github.com/yudai/gotty>.

#### Share result of command:
```shell
gotty {{command}}
```
#### Share with write permission:
```shell
gotty -w {{shell}}
```
#### Share with credential (Basic Auth):
```shell
gotty -w -c {{username}}:{{password}} {{shell}}
```
{% endraw %}