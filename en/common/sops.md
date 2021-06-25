---
layout: default
title: "sops"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sops">
  <a href="/en/common/sops.html">sops</a> <a href="#sops"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SOPS: Secrets OPerationS.
> Tool for managing secrets.
> More information: <https://github.com/mozilla/sops>.

#### Encrypt a file:
```shell
sops -e {{path/to/myfile.json}} > {{path/to/myfile.enc.json}}
```
#### Decrypt a file to the standard output:
```shell
sops -d {{path/to/myfile.enc.json}}
```
#### Rotate data keys for a sops file:
```shell
sops -r {{path/to/myfile.enc.yaml}}
```
#### Change the extension of the file once encrypted:
```shell
sops -d --input-type json {{path/to/myfile.enc.json}}
```
#### Extract keys by naming them, and array elements by numbering them:
```shell
sops -d --extract '["an_array"][1]' {{path/to/myfile.enc.json}}
```
#### Show the difference between two sops files:
```shell
diff <(sops -d {{path/to/secret1.enc.yaml}}) <(sops -d {{path/to/secret2.enc.yaml}})
```
{% endraw %}