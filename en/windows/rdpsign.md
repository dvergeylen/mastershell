---
layout: default
title: "rdpsign"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rdpsign">
  <a href="/en/windows/rdpsign.html">rdpsign</a> <a href="#rdpsign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for signing Remote Desktop Protocol (RDP) files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/rdpsign>.

#### Sign an RDP file:
```shell
rdpsign {{path/to/file.rdp}}
```
#### Sign an RDP file using a specific sha256 hash:
```shell
rdpsign {{path/to/file.rdp}} /sha265 {{hash}}
```
#### Enable quiet output:
```shell
rdpsign {{path/to/file.rdp}} /q
```
#### Display verbose warnings, messages and statuses:
```shell
rdpsign {{path/to/file.rdp}} /v
```
#### Test the signing by displaying the output to stdout without updating the file:
```shell
rdpsign {{path/to/file.rdp}} /l
```
{% endraw %}