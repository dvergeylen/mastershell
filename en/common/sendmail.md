---
layout: default
title: "sendmail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sendmail">
  <a href="/en/common/sendmail.html">sendmail</a> <a href="#sendmail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send email from the command-line.

#### Send a message with the content of `message.txt` to the mail directory of local user `username`:
```shell
sendmail {{username}} < {{message.txt}}
```
#### Send an email from you@yourdomain.com (assuming the mail server is configured for this) to test@gmail.com containing the message in `message.txt`:
```shell
sendmail -f {{you@yourdomain.com}} {{test@gmail.com}} < {{message.txt}}
```
#### Send an email from you@yourdomain.com (assuming the mail server is configured for this) to test@gmail.com containing the file `file.zip`:
```shell
sendmail -f {{you@yourdomain.com}} {{test@gmail.com}} < {{file.zip}}
```
{% endraw %}