---
layout: default
title: "tmpmail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tmpmail">
  <a href="/en/common/tmpmail.html">tmpmail</a> <a href="#tmpmail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A temporary email right from your terminal written in POSIX sh.
> More information: <https://github.com/sdushantha/tmpmail>.

#### Create a temporary inbox:
```shell
tmpmail --generate
```
#### List messages and their numeric ID:
```shell
tmpmail
```
#### Display the most recent received email:
```shell
tmpmail --recent
```
#### Open a specific message:
```shell
tmpmail {{email_id}}
```
#### View email as raw text without HTML tags:
```shell
tmpmail --text
```
#### Open email with a specific browser (default is w3m):
```shell
tmpmail --browser {{browser}}
```
{% endraw %}