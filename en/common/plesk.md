---
layout: default
title: "plesk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="plesk">
  <a href="/en/common/plesk.html">plesk</a> <a href="#plesk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Plesk hosting control panel CLI interface.
> More information: <https://docs.plesk.com>.

#### Generate an auto login link for the admin user and print it:
```shell
plesk login
```
#### Show product version information:
```shell
plesk version
```
#### List all hosted domains:
```shell
plesk bin domain --list
```
#### Start watching for changes in the `panel.log` file:
```shell
plesk log {{panel.log}}
```
#### Start the interactive MySQL console:
```shell
plesk db
```
#### Open the Plesk main configuration file in the default editor:
```shell
plesk conf {{panel.ini}}
```
{% endraw %}