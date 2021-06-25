---
layout: default
title: "lastcomm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lastcomm">
  <a href="/en/linux/lastcomm.html">lastcomm</a> <a href="#lastcomm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show last commands executed.
> More information: <https://manpages.debian.org/stable/acct/lastcomm.1.en.html>.

#### Print information about all of the commands in the acct (record file):
```shell
lastcomm
```
#### Display commands executed by a given user:
```shell
lastcomm --user {{user}}
```
#### Display information about a given command executed on the system:
```shell
lastcomm --command {{command}}
```
#### Display information about commands executed on a given terminal:
```shell
lastcomm --tty {{terminal_name}}
```
{% endraw %}