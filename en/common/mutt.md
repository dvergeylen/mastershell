---
layout: default
title: "mutt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mutt">
  <a href="/en/common/mutt.html">mutt</a> <a href="#mutt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line email client.
> More information: <http://mutt.org>.

#### Open the specified mailbox:
```shell
mutt -f {{mailbox}}
```
#### Send an email and specify a subject and a cc recipient:
```shell
mutt -s {{subject}} -c {{cc@example.com}} {{recipient@example.com}}
```
#### Send an email with files attached:
```shell
mutt -a {{file1}} {{file2}} -- {{recipient@example.com}}
```
#### Specify a file to include as the message body:
```shell
mutt -i {{file}} {{recipient@example.com}}
```
#### Specify a draft file containing the header and the body of the message, in RFC 5322 format:
```shell
mutt -H {{file}} {{recipient@example.com}}
```
{% endraw %}