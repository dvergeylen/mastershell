---
layout: default
title: "prctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="prctl">
  <a href="/en/sunos/prctl.html">prctl</a> <a href="#prctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get or set the resource controls of running processes,.
> Tasks, and projects.
> More information: <https://www.unix.com/man-page/sunos/1/prctl>.

#### Examine process limits and permissions:
```shell
prctl {{PID}}
```
#### Examine process limits and permissions in machine parseable format:
```shell
prctl -P {{PID}}
```
#### Get specific limit for a running process:
```shell
prctl -n process.max-file-descriptor {{PID}}
```
{% endraw %}