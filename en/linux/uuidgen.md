---
layout: default
title: "uuidgen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uuidgen">
  <a href="/en/linux/uuidgen.html">uuidgen</a> <a href="#uuidgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate unique identifiers (UUIDs).
> See also `uuid`.
> More information: <https://manned.org/uuidgen>.

#### Create a random UUIDv4:
```shell
uuidgen --random
```
#### Create a UUIDv1 based on the current time:
```shell
uuidgen --time
```
#### Create a UUIDv5 of the name with a specified namespace prefix:
```shell
uuidgen --sha1 --namespace {{@dns|@url|@oid|@x500}} --name {{object_name}}
```
{% endraw %}