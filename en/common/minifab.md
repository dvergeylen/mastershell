---
layout: default
title: "minifab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="minifab">
  <a href="/en/common/minifab.html">minifab</a> <a href="#minifab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility tool that automates the setup and deployment of Hyperledger Fabric networks.
> More information: <https://github.com/hyperledger-labs/minifabric>.

#### Bring up the default Hyperledger Fabric network:
```shell
minifab up -i {{minifab_version}}
```
#### Bring down the Hyperledger Fabric network:
```shell
minifab down
```
#### Install chaincode onto a specified channel:
```shell
minifab install -n {{chaincode_name}}
```
#### Install a specific chaincode version onto a channel:
```shell
minifab install -n {{chaincode_name}} -v {{chaincode_version}}
```
#### Initialize the chaincode after installation/upgrade:
```shell
minifab approve,commit,initialize,discover
```
#### Invoke a chaincode method with the specified arguments:
```shell
minifab invoke -n {{chaincode_name}} -p '"{{method_name}}", "{{arg0}}", "{{arg1}}", ...'
```
#### Make a query on the ledger:
```shell
minifab blockquery {{block_number}}
```
#### Quickly run an application:
```shell
minifab apprun -l {{app_programming_langauge}}
```
{% endraw %}