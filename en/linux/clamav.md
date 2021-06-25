---
layout: default
title: "clamav"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clamav">
  <a href="/en/linux/clamav.html">clamav</a> <a href="#clamav"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open-source anti-virus program.
> Designed especially for e-mail scanning on mail gateways, but can be used in other contexts.
> More information: <https://www.clamav.net>.

#### Update virus definitions:
```shell
freshclam
```
#### Scan a file for viruses:
```shell
clamscan {{path/to/file}}
```
#### Scan directories recursively and print out infected files:
```shell
clamscan --recursive --infected {{path/to/directory}}
```
#### Scan directories recursively and move them into quarantine:
```shell
clamscan --recursive --move={{directory}}
```
{% endraw %}