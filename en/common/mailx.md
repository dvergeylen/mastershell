---
layout: default
title: "mailx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mailx">
  <a href="/en/common/mailx.html">mailx</a> <a href="#mailx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send and receive mail.

#### Send mail (the content should be typed after the command, and ended with `Ctrl+D`):
```shell
mailx -s "{{subject}}" {{to_addr}}
```
#### Send mail with content passed from another command:
```shell
echo "{{content}}" | mailx -s "{{subject}}" {{to_addr}}
```
#### Send mail with content read from a file:
```shell
mailx -s "{{subject}}" {{to_addr}} < {{content.txt}}
```
#### Send mail to a recipient and CC to another address:
```shell
mailx -s "{{subject}}" -c {{cc_addr}} {{to_addr}}
```
#### Send mail specifying the sender address:
```shell
mailx -s "{{subject}}" -r {{from_addr}} {{to_addr}}
```
#### Send mail with an attachment:
```shell
mailx -a {{file}} -s "{{subject}}" {{to_addr}}
```
{% endraw %}