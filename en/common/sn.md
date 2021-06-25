---
layout: default
title: "sn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sn">
  <a href="/en/common/sn.html">sn</a> <a href="#sn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mono StrongName utility for signing and verifying IL assemblies.

#### Generate a new StrongNaming key:
```shell
sn -k {{path/to/key.snk}}
```
#### Re-sign an assembly with the specified private key:
```shell
sn -R {{path/to/assembly.dll}} {{path/to/key_pair.snk}}
```
#### Show the public key of the private key that was used to sign an assembly:
```shell
sn -T {{path/to/assembly.exe}}
```
#### Extract the public key to a file:
```shell
sn -e {{path/to/assembly.dll}} {{path/to/output.pub}}
```
{% endraw %}