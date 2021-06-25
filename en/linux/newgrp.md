---
layout: default
title: "newgrp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="newgrp">
  <a href="/en/linux/newgrp.html">newgrp</a> <a href="#newgrp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Switch primary group membership.

#### Change user's primary group membership:
```shell
newgrp {{group_name}}
```
#### Reset primary group membership to user's default group in `/etc/passwd`:
```shell
newgrp
```
{% endraw %}