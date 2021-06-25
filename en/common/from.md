---
layout: default
title: "from"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="from">
  <a href="/en/common/from.html">from</a> <a href="#from"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prints mail header lines from the current user's mailbox.
> More information: <https://mailutils.org/manual/html_chapter/Programs.html#frm-and-from>.

#### List mail:
```shell
from
```
#### Display the number of messages stored:
```shell
from --count
```
#### List mail in the specified mailbox directory:
```shell
MAIL={{path/to/mailbox}} from
```
#### Print the mail from the specified address:
```shell
from --sender={{me@example.com}}
```
{% endraw %}