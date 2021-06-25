---
layout: default
title: "imapsync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="imapsync">
  <a href="/en/common/imapsync.html">imapsync</a> <a href="#imapsync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Email IMAP tool for syncing, copying and migrating email mailboxes between two imap servers, one way, and without duplicates.
> More information: <https://imapsync.lamiral.info>.

#### Synchronize imap account between host1 and host2:
```shell
imapsync --host1 {{host1}} --user1 {{user1}} --password1 {{secret1}} --host2 {{host2}} --user2 {{user2}} --password2 {{secret2}}
```
{% endraw %}