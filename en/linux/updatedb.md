---
layout: default
title: "updatedb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="updatedb">
  <a href="/en/linux/updatedb.html">updatedb</a> <a href="#updatedb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create or update the database used by `locate`.
> It is usually run daily by cron.

#### Refresh database content:
```shell
sudo updatedb
```
#### Display file names as soon as they are found:
```shell
sudo updatedb --verbose
```
{% endraw %}