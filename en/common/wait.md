---
layout: default
title: "wait"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wait">
  <a href="/en/common/wait.html">wait</a> <a href="#wait"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wait for a process to complete before proceeding.

#### Wait for a process to finish given its process ID (PID) and return its exit status:
```shell
wait {{pid}}
```
#### Wait for all processes known to the invoking shell to finish:
```shell
wait
```
{% endraw %}