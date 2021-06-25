---
layout: default
title: "snmpwalk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="snmpwalk">
  <a href="/en/linux/snmpwalk.html">snmpwalk</a> <a href="#snmpwalk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SNMP query tool.
> More information: <https://manned.org/snmpwalk>.

#### Query the system information of a remote host using SNMPv1 and a community string:
```shell
snmpwalk -v1 -c {{community}} {{ip}}
```
#### Query specific system information on a remote host by OID using SNMPv2 on a specified port:
```shell
snmpwalk -v2c -c {{community}} {{ip}}:{{port}} {{oid}}
```
#### Query specific system information on a remote host by OID using SNMPv3 and authentication without encryption:
```shell
snmpwalk -v3 -l {{authNoPriv}} -u {{username}} -a {{MD5|SHA}} -A {{passphrase}} {{ip}} {{oid}}
```
#### Query specific system information on a remote host by OID using SNMPv3, authentication, and encryption:
```shell
snmpwalk -v3 -l {{authPriv}} -u {{username}} -a {{MD5|SHA}} -A {{auth_passphrase}} -x {{DES|AES}} -X {{enc_passphrase}} {{ip}} {{oid}}
```
#### Query specific system information on a remote host by OID using SNMPv3 without authentication or encryption:
```shell
snmpwalk -v3 -l {{noAuthNoPriv}} -u {{username}} {{ip}} {{oid}}
```
{% endraw %}