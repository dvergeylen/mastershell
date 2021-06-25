---
layout: default
title: "rmdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rmdir">
  <a href="/nl/windows/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwijdert een directory en zijn inhoud.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/rmdir>.

#### Verwijder een lege directory:
```shell
rmdir {{pad/naar/directory}}
```
#### verwijder een directory en zen inhoud recursief:
```shell
rmdir {{pad/naar/directory}} /s
```
#### verwijder een directory en zen inhoud recursief zonder te vragen:
```shell
rmdir {{pad/naar/directory}} /s /q
```
{% endraw %}