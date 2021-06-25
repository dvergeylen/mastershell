---
layout: default
title: "keybase"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="keybase">
  <a href="/en/common/keybase.html">keybase</a> <a href="#keybase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Key directory that maps social media identities to encryption keys in a publicly auditable manner.
> More information: <https://keybase.io/docs/command_line>.

#### Follow another user:
```shell
keybase follow {{username}}
```
#### Add a new proof:
```shell
keybase prove {{service}} {{service_username}}
```
#### Sign a file:
```shell
keybase sign --infile {{input_file}} --outfile {{output_file}}
```
#### Verify a signed file:
```shell
keybase verify --infile {{input_file}} --outfile {{output_file}}
```
#### Encrypt a file:
```shell
keybase encrypt --infile {{input_file}} --outfile {{output_file}} {{receiver}}
```
#### Decrypt a file:
```shell
keybase decrypt --infile {{input_file}} --outfile {{output_file}}
```
#### Revoke current device, log out, and delete local data:
```shell
keybase deprovision
```
{% endraw %}