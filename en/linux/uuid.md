---
layout: default
title: "uuid"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uuid">
  <a href="/en/linux/uuid.html">uuid</a> <a href="#uuid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate and decode Universally Unique Identifiers (UUID).
> See also `uuidgen`.
> More information: <https://manned.org/uuid>.

#### Generate a UUIDv1 (based on time and system's hardware address, if present):
```shell
uuid
```
#### Generate a UUIDv4 (based on random data):
```shell
uuid -v {{4}}
```
#### Generate multiple UUIDv4 identifiers at once:
```shell
uuid -v {{4}} -n {{number_of_uuids}}
```
#### Generate a UUIDv4 and specify the output format:
```shell
uuid -v {{4}} -F {{BIN|STR|SIV}}
```
#### Generate a UUIDv4 and write the output to a file:
```shell
uuid -v {{4}} -o {{path/to/file}}
```
#### Generate a UUIDv5 (based on the supplied object name) with a specified namespace prefix:
```shell
uuid -v {{5}} ns:{{DNS|URL|OID|X500}} {{object_name}}
```
#### Decode a given UUID:
```shell
uuid -d {{uuid}}
```
{% endraw %}