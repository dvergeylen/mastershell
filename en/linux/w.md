---
layout: default
title: "w"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="w">
  <a href="/en/linux/w.html">w</a> <a href="#w"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display who is logged in and their processes.
> More information: <https://www.geeksforgeeks.org/w-command-in-linux-with-examples/>.

#### Display information about all users who are currently logged in:
```shell
w
```
#### Display information about a specific user:
```shell
w {{user}}
```
#### Display information without including the header:
```shell
w --no-header
```
#### Display information without including the login, JCPU and PCPU columns:
```shell
w --short
```
{% endraw %}