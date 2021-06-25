---
layout: default
title: "sfc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sfc">
  <a href="/en/windows/sfc.html">sfc</a> <a href="#sfc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scans the integrity of Windows system files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/sfc>.

#### Display information about the usage of the command:
```shell
sfc
```
#### Scan all system files and, if possible, repair any problems:
```shell
sfc /scannow
```
#### Scan all system files without attempting to repair any:
```shell
sfc /verifyonly
```
#### Scan a specific file and, if possible, repair any problems:
```shell
sfc /scanfile={{path/to/file}}
```
#### Scan a specific file without attempting to repair it:
```shell
sfc /verifyfile={{path/to/file}}
```
#### When repairing offline, specify the boot directory:
```shell
sfc /offbootdir={{path/to/directory}}
```
#### When repairing offline, specify the Windows directory:
```shell
sfc /offwindir={{path/to/directory}}
```
{% endraw %}