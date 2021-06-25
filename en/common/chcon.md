---
layout: default
title: "chcon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chcon">
  <a href="/en/common/chcon.html">chcon</a> <a href="#chcon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change SELinux security context of a file or files/directories.
> More information: <https://www.gnu.org/software/coreutils/chcon>.

#### View security context of a file:
```shell
ls -lZ {{path/to/file}}
```
#### Change the security context of a target file, using a reference file:
```shell
chcon --reference={{reference_file}} {{target_file}}
```
#### Change the full SELinux security context of a file:
```shell
chcon {{user}}:{{role}}:{{type}}:{{range/level}} {{filename}}
```
#### Change only the user part of SELinux security context:
```shell
chcon -u {{user}} {{filename}}
```
#### Change only the role part of SELinux security context:
```shell
chcon -r {{role}} {{filename}}
```
#### Change only the type part of SELinux security context:
```shell
chcon -t {{type}} {{filename}}
```
#### Change only the range/level part of SELinux security context:
```shell
chcon -l {{range/level}} {{filename}}
```
{% endraw %}