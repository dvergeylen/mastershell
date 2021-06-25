---
layout: default
title: "initdb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="initdb">
  <a href="/en/common/initdb.html">initdb</a> <a href="#initdb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a PostgreSQL database on disk.
> More information: <https://www.postgresql.org/docs/9.5/app-initdb.html>.

#### Create a database at `/usr/local/var/postgres`:
```shell
initdb -D /usr/local/var/postgres
```
{% endraw %}