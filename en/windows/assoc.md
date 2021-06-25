---
layout: default
title: "assoc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="assoc">
  <a href="/en/windows/assoc.html">assoc</a> <a href="#assoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or modify file extension associations.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/assoc>.

#### Display all associated filetypes:
```shell
assoc
```
#### Display the associated filetype for a specific extension:
```shell
assoc {{.txt}}
```
#### Modify the associated filetype for a specific extension:
```shell
assoc {{.txt}}={{txtfile}}
```
{% endraw %}