---
layout: default
title: "repair-bde"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="repair-bde">
  <a href="/en/windows/repair-bde.html">repair-bde</a> <a href="#repair-bde"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Attempt to repair or decrypt a damaged BitLocker-encrypted volume.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/repair-bde>.

#### Attempt to repair a specified volume:
```shell
repair-bde {{C:}}
```
#### Attempt to repair a specified volume and output to another volume:
```shell
repair-bde {{C:}} {{D:}}
```
#### Attempt to repair a specified volume using the provided recovery key file:
```shell
repair-bde {{C:}} -RecoveryKey {{path/to/file.bek}}
```
#### Attempt to repair a specified volume using the provided numerical recovery password:
```shell
repair-bde {{C:}} -RecoveryPassword {{password}}
```
#### Attempt to repair a specified volume using the provided password:
```shell
repair-bde {{C:}} -Password {{password}}
```
#### Attempt to repair a specified volume using the provided key package:
```shell
repair-bde {{C:}} -KeyPackage {{path/to/directory}}
```
#### Log all output to a specific file:
```shell
repair-bde {{C:}} -LogFile {{path/to/file}}
```
#### Display all available options:
```shell
repair-bde /?
```
{% endraw %}