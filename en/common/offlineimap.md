---
layout: default
title: "offlineimap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="offlineimap">
  <a href="/en/common/offlineimap.html">offlineimap</a> <a href="#offlineimap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Synchronize a remote IMAP server with local Maildir folders.
> More information: <http://www.offlineimap.org>.

#### Synchronize once, without enabling autorefresh:
```shell
offlineimap -o
```
#### Synchronize a specific account:
```shell
offlineimap -a {{account}}
```
#### Synchronize a specific folder:
```shell
offlineimap -f {{folder}}
```
{% endraw %}