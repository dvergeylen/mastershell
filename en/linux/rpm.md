---
layout: default
title: "rpm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rpm">
  <a href="/en/linux/rpm.html">rpm</a> <a href="#rpm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> RPM Package Manager.

#### Show version of httpd package:
```shell
rpm -q {{httpd}}
```
#### List versions of all matching packages:
```shell
rpm -qa '{{mariadb*}}'
```
#### Forcibly install a package regardless of currently installed versions:
```shell
rpm -U {{package_name.rpm}} --force
```
#### Identify owner of a file and show version of the package:
```shell
rpm -qf {{/etc/postfix/main.cf}}
```
#### List package-owned files:
```shell
rpm -ql {{kernel}}
```
#### Show scriptlets from an RPM file:
```shell
rpm -qp --scripts {{package_name.rpm}}
```
#### Show changed, missing and/or incorrectly installed files of matching packages:
```shell
rpm -Va '{{php-*}}'
```
{% endraw %}