---
layout: default
title: "hello"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hello">
  <a href="/en/linux/hello.html">hello</a> <a href="#hello"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print "Hello, world!", "hello, world" or a customizable text.
> More information: <https://www.gnu.org/software/hello/>.

#### Print "Hello, world!":
```shell
hello
```
#### Print "hello, world", the traditional type:
```shell
hello --traditional
```
#### Print a text message:
```shell
hello --greeting="{{greeting_text}}"
```
{% endraw %}