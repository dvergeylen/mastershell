---
layout: default
title: "ldapsearch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ldapsearch">
  <a href="/en/common/ldapsearch.html">ldapsearch</a> <a href="#ldapsearch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI utility for querying an LDAP directory.

#### Query an LDAP server for all items that are a member of the given group and return the object's displayName value:
```shell
ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} -b {{base_ou}} '{{memberOf=group1}}' displayName
```
#### Query an LDAP server with a no-newline password file for all items that are a member of the given group and return the object's displayName value:
```shell
ldapsearch -D '{{admin_DN}}' -y '{{password_file}}' -h {{ldap_host}} -b {{base_ou}} '{{memberOf=group1}}' displayName
```
#### Return 5 items that match the given filter:
```shell
ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} -b {{base_ou}} '{{memberOf=group1}}' -z 5 displayName
```
#### Wait up to 7 seconds for a response:
```shell
ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} -b {{base_ou}} '{{memberOf=group1}}' -l 7 displayName
```
#### Invert the filter:
```shell
ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} -b {{base_ou}} '(!(memberOf={{group1}}))' displayName
```
#### Return all items that are part of multiple groups, returning the display name for each item:
```shell
ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} '(&({{memberOf=group1}})({{memberOf=group2}})({{memberOf=group3}}))' "displayName"
```
#### Return all items that are members of at least 1 of the specified groups:
```shell
ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} '(|({{memberOf=group1}})({{memberOf=group1}})({{memberOf=group3}}))' displayName
```
#### Combine multiple boolean logic filters:
```shell
ldapsearch -D '{{admin_DN}}' -w '{{password}}' -h {{ldap_host}} '(&({{memberOf=group1}})({{memberOf=group2}})(!({{memberOf=group3}})))' displayName
```
{% endraw %}