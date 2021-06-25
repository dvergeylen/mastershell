---
layout: default
title: "lp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lp">
  <a href="/en/common/lp.html">lp</a> <a href="#lp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print files.

#### Print the output of a command to the default printer (see `lpstat` command):
```shell
echo "test" | lp
```
#### Print a file to the default printer:
```shell
lp {{path/to/filename}}
```
#### Print a file to a named printer (see `lpstat` command):
```shell
lp -d {{printer_name}} {{path/to/filename}}
```
#### Print N copies of file to default printer (replace N with desired number of copies):
```shell
lp -n {{N}} {{path/to/filename}}
```
#### Print only certain pages to the default printer (print pages 1, 3-5, and 16):
```shell
lp -P 1,3-5,16 {{path/to/filename}}
```
#### Resume printing a job:
```shell
lp -i {{job_id}} -H resume
```
{% endraw %}