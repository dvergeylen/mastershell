---
layout: default
title: "shift"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shift">
  <a href="/en/common/shift.html">shift</a> <a href="#shift"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bash built-in command that shifts the arguments passed to the calling function or script by a specified number of places.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#index-shift>.

#### Move arguments by one place dropping the first argument:
```shell
shift
```
#### Move arguments by N places dropping the first N arguments:
```shell
shift {{N}}
```
{% endraw %}